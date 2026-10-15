---
title: "GetText"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mengekstrak teks dari dokumen."
type: docs
weight: 180
url: /id/net/groupdocs.parser/parser/gettext/
---

## GetText() {#gettext}

Mengekstrak teks dari dokumen.

```csharp
public TextReader GetText()
```

### Nilai Kembali

Sebuah instance dari kelas TextReader dengan teks yang diekstrak; `null` jika ekstraksi teks tidak didukung.

### Catatan

**Learn more:**

* [Extract text from documents](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Contoh

Contoh berikut menunjukkan cara mengekstrak teks dari dokumen:

```csharp
// Buat sebuah instance dari kelas Parser
using(Parser parser = new Parser(filePath))
{
    // Ekstrak teks ke dalam pembaca
    using(TextReader reader = parser.GetText())
    {
        // Cetak teks dari dokumen
        // Jika ekstraksi teks tidak didukung, pembaca akan bernilai null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Lihat Juga

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(TextOptions) {#gettext_1}

Mengekstrak halaman teks dari dokumen menggunakan opsi teks (untuk mengaktifkan mode ekstraksi teks mentah cepat).

```csharp
public TextReader GetText(TextOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| options | TextOptions | Opsi ekstraksi teks. |

### Nilai Kembali

Sebuah instance dari kelas TextReader dengan teks yang diekstrak; `null` jika ekstraksi teks tidak didukung.

### Catatan

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Contoh

Contoh berikut menunjukkan cara mengekstrak teks mentah dari dokumen:

```csharp
// Buat sebuah instance dari kelas Parser
using(Parser parser = new Parser(filePath))
{
    // Ekstrak teks mentah ke dalam pembaca
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // Cetak teks dari dokumen
        // Jika ekstraksi teks tidak didukung, pembaca akan bernilai null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Lihat Juga

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

Mengekstrak teks dari halaman dokumen.

```csharp
public TextReader GetText(int pageIndex)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| pageIndex | Int32 | Indeks halaman berbasis nol. |

### Nilai Kembali

Sebuah instance dari kelas TextReader dengan teks yang diekstrak; `null` jika ekstraksi halaman teks tidak didukung.

### Catatan

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Contoh

Contoh berikut menunjukkan cara mengekstrak teks dari halaman dokumen:

```csharp
// Buat sebuah instance dari kelas Parser
using(Parser parser = new Parser(filePath))
{
    // Periksa apakah dokumen mendukung ekstraksi teks
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Dapatkan informasi dokumen
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Periksa apakah dokumen memiliki halaman
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Iterasi melalui halaman
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // Cetak nomor halaman 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // Ekstrak teks ke dalam pembaca
        using(TextReader reader = parser.GetText(p))
        {
            // Cetak teks dari dokumen
            // Kami mengabaikan pengecekan null karena kami telah memeriksa dukungan fitur ekstraksi teks sebelumnya
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Lihat Juga

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(int, TextOptions) {#gettext_3}

Mengekstrak teks dari halaman dokumen menggunakan opsi teks (untuk mengaktifkan mode ekstraksi teks mentah cepat).

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| pageIndex | Int32 | Indeks halaman berbasis nol. |
| options | TextOptions | Opsi ekstraksi teks. |

### Nilai Kembali

Sebuah instance dari kelas TextReader dengan teks yang diekstrak; `null` jika ekstraksi halaman teks tidak didukung.

### Catatan

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Contoh

Contoh berikut menunjukkan cara mengekstrak teks mentah dari halaman dokumen:

```csharp
// Buat sebuah instance dari kelas Parser
using(Parser parser = new Parser(filePath))
{
    // Periksa apakah dokumen mendukung ekstraksi teks
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Dapatkan informasi dokumen
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // Periksa apakah dokumen memiliki halaman
    if(documentInfo == null || documentInfo.RawPageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Iterasi melalui halaman
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // Cetak nomor halaman 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // Ekstrak teks ke dalam pembaca
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // Cetak teks dari dokumen
            // Kami mengabaikan pengecekan null karena kami telah memeriksa dukungan fitur ekstraksi teks sebelumnya
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Lihat Juga

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->

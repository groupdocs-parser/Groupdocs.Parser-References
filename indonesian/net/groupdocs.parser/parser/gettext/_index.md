---
title: GetText
second_title: GroupDocs.Parser untuk Referensi .NET API
description: Mengekstrak teks dari dokumen.
type: docs
weight: 150
url: /id/net/groupdocs.parser/parser/gettext/
---
## GetText() {#gettext}

Mengekstrak teks dari dokumen.

```csharp
public TextReader GetText()
```

### Nilai Pengembalian

Contoh dariTextReader kelas dengan teks yang diekstrak; `batal` jika ekstraksi teks tidak didukung.

### Perkataan

**Belajarlah lagi:**

* [Ekstrak teks dari dokumen](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [Ekstrak teks dalam mode Akurat](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Contoh

Contoh berikut menunjukkan cara mengekstrak teks dari dokumen:

```csharp
// Buat instance dari kelas Parser
using(Parser parser = new Parser(filePath))
{
    // Ekstrak teks ke pembaca
    using(TextReader reader = parser.GetText())
    {
        // Cetak teks dari dokumen
        // Jika ekstraksi teks tidak didukung, pembaca adalah null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Lihat juga

* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## GetText(TextOptions) {#gettext_1}

Mengekstrak halaman teks dari dokumen menggunakan opsi teks (untuk mengaktifkan mode ekstraksi teks cepat mentah).

```csharp
public TextReader GetText(TextOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| options | TextOptions | Opsi ekstraksi teks. |

### Nilai Pengembalian

Contoh dariTextReader kelas dengan teks yang diekstrak; `batal` jika ekstraksi teks tidak didukung.

### Perkataan

**Belajarlah lagi:**

* [Ekstrak teks dalam mode Akurat](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Ekstrak teks dalam mode Raw](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Contoh

Contoh berikut menunjukkan cara mengekstrak teks mentah dari dokumen:

```csharp
// Buat instance dari kelas Parser
using(Parser parser = new Parser(filePath))
{
    // Ekstrak teks mentah ke pembaca
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // Cetak teks dari dokumen
        // Jika ekstraksi teks tidak didukung, pembaca adalah null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Lihat juga

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

Mengekstrak teks dari halaman dokumen.

```csharp
public TextReader GetText(int pageIndex)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| pageIndex | Int32 | Indeks halaman berbasis nol. |

### Nilai Pengembalian

Contoh dariTextReader kelas dengan teks yang diekstrak; `batal` jika ekstraksi halaman teks tidak didukung.

### Perkataan

**Belajarlah lagi:**

* [Ekstrak teks dalam mode Akurat](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Contoh

Contoh berikut menunjukkan cara mengekstrak teks dari halaman dokumen:

```csharp
// Buat instance dari kelas Parser
using(Parser parser = new Parser(filePath))
{
    // Periksa apakah dokumen mendukung ekstraksi teks
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Dapatkan info dokumen
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Periksa apakah dokumen memiliki halaman
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Ulangi beberapa halaman
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // Cetak nomor halaman 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // Ekstrak teks ke pembaca
        using(TextReader reader = parser.GetText(p))
        {
            // Cetak teks dari dokumen
            // Kami mengabaikan pemeriksaan nol karena kami telah memeriksa dukungan fitur ekstraksi teks sebelumnya
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Lihat juga

* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## GetText(int, TextOptions) {#gettext_3}

Mengekstrak teks dari halaman dokumen menggunakan opsi teks (untuk mengaktifkan mode ekstraksi teks cepat mentah).

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| pageIndex | Int32 | Indeks halaman berbasis nol. |
| options | TextOptions | Opsi ekstraksi teks. |

### Nilai Pengembalian

Contoh dariTextReader kelas dengan teks yang diekstrak; `batal` jika ekstraksi halaman teks tidak didukung.

### Perkataan

**Belajarlah lagi:**

* [Ekstrak teks dalam mode Akurat](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Ekstrak teks dalam mode Raw](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Contoh

Contoh berikut menunjukkan cara mengekstrak teks mentah dari halaman dokumen:

```csharp
// Buat instance dari kelas Parser
using(Parser parser = new Parser(filePath))
{
    // Periksa apakah dokumen mendukung ekstraksi teks
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Dapatkan info dokumen
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // Periksa apakah dokumen memiliki halaman
    if(documentInfo == null || documentInfo.RawPageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Ulangi beberapa halaman
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // Cetak nomor halaman 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // Ekstrak teks ke pembaca
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // Cetak teks dari dokumen
            // Kami mengabaikan pemeriksaan nol karena kami telah memeriksa dukungan fitur ekstraksi teks sebelumnya
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Lihat juga

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

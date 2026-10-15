---
title: "GetFormattedText"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mengekstrak teks terformat dari dokumen."
type: docs
weight: 100
url: /id/net/groupdocs.parser/parser/getformattedtext/
---

## GetFormattedText(FormattedTextOptions) {#getformattedtext}

Mengekstrak teks terformat dari dokumen.

```csharp
public TextReader GetFormattedText(FormattedTextOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| options | FormattedTextOptions | Opsi ekstraksi teks terformat. |

### Nilai Kembali

Sebuah instance dari kelas TextReader dengan teks yang diekstrak; `null` jika ekstraksi teks terformat tidak didukung.

### Catatan

**Learn more:**

* [Extract formatted text from document](https://docs.groupdocs.com/display/parsernet/Extract+formatted+text+from+document)
* Extract a document text as [HTML](https://docs.groupdocs.com/display/parsernet/HTML)
* Extract a document text as [Markdown](https://docs.groupdocs.com/display/parsernet/Markdown)
* Extract a document text as [Plain text](https://docs.groupdocs.com/display/parsernet/Plain+text)

### Contoh

Contoh berikut menunjukkan cara mengekstrak teks dokumen sebagai teks HTML:

```csharp
// Buat sebuah instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Ekstrak teks terformat ke dalam pembaca
    using (TextReader reader = parser.GetFormattedText(new FormattedTextOptions(FormattedTextMode.Html)))
    {
        // Cetak teks terformat dari dokumen
        // Jika ekstraksi teks terformat tidak didukung, pembaca akan bernilai null
        Console.WriteLine(reader == null ? "Formatted text extraction isn't suppported" : reader.ReadToEnd());
    }
}
```

### Lihat Juga

* class [FormattedTextOptions](../../../groupdocs.parser.options/formattedtextoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetFormattedText(int, FormattedTextOptions) {#getformattedtext_1}

Mengekstrak teks terformat dari halaman dokumen.

```csharp
public TextReader GetFormattedText(int pageIndex, FormattedTextOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| pageIndex | Int32 | Indeks halaman berbasis nol. |
| options | FormattedTextOptions | Opsi ekstraksi teks terformat. |

### Nilai Kembali

Sebuah instance dari kelas TextReader dengan teks yang diekstrak; `null` jika ekstraksi halaman teks terformat tidak didukung.

### Catatan

**Learn more:**

* [Extract formatted text from document page](https://docs.groupdocs.com/display/parsernet/Extract+formatted+text+from+document+page)
* Extract a document text as [HTML](https://docs.groupdocs.com/display/parsernet/HTML)
* Extract a document text as [Markdown](https://docs.groupdocs.com/display/parsernet/Markdown)
* Extract a document text as [Plain text](https://docs.groupdocs.com/display/parsernet/Plain+text)

### Contoh

Contoh berikut menunjukkan cara mengekstrak teks halaman dokumen sebagai teks Markdown:

```csharp
// Buat sebuah instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Periksa apakah dokumen mendukung ekstraksi teks terformat
    if (!parser.Features.FormattedText)
    {
        Console.WriteLine("Document isn't supports formatted text extraction.");
        return;
    }
    
    // Dapatkan informasi dokumen
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Periksa apakah dokumen memiliki halaman
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // Iterasi melalui halaman
    for (int p = 0; p<documentInfo.PageCount; p++)
    {
        // Cetak nomor halaman 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
        // Ekstrak teks terformat ke dalam pembaca
        using (TextReader reader = parser.GetFormattedText(p, new FormattedTextOptions(FormattedTextMode.Markdown)))
        {
            // Cetak teks terformat dari dokumen
            // Kami mengabaikan pemeriksaan null karena kami telah memeriksa dukungan fitur ekstraksi teks terformat sebelumnya
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Lihat Juga

* class [FormattedTextOptions](../../../groupdocs.parser.options/formattedtextoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->

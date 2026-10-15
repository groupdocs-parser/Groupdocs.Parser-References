---
title: "ExtractText"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mengekstrak teks dari dokumen yang dirujuk oleh objek TocItemgroupdocs.parser.data/tocitem."
type: docs
weight: 50
url: /id/net/groupdocs.parser.data/tocitem/extracttext/
---

## TocItem.ExtractText method

Mengekstrak teks dari dokumen yang dirujuk oleh objek [`TocItem`](../../tocitem).

```csharp
public virtual TextReader ExtractText()
```

### Nilai Kembali

Sebuah instance dari kelas TextReader dengan teks yang diekstrak.

### Contoh

Contoh berikut cara mengekstrak teks menggunakan item dari daftar isi:

```csharp
// Buat sebuah instance dari kelas Parser
using (Parser parser = new Parser(Constants.SampleDocxWithToc))
{
    // Dapatkan daftar isi
    IEnumerable<TocItem> tocItems = parser.GetToc();
    // Periksa apakah ekstraksi toc didukung
    if (tocItems == null)
    {
        Console.WriteLine("Table of contents extraction isn't supported");
    }
    // Iterasi pada item
    foreach (TocItem tocItem in tocItems)
    {
        // Cetak teks bab
        using (TextReader reader = tocItem.ExtractText())
        {
            Console.WriteLine("----");
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Lihat Juga

* class [TocItem](../../tocitem)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->

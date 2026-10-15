---
title: "GetToc"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mengekstrak daftar isi dari dokumen."
type: docs
weight: 200
url: /id/net/groupdocs.parser/parser/gettoc/
---

## Parser.GetToc method

Mengekstrak daftar isi dari dokumen.

```csharp
public IEnumerable<TocItem> GetToc()
```

### Nilai Kembali

Koleksi item daftar isi; `null` jika ekstraksi daftar isi tidak didukung.

### Catatan

**Learn more:**

* [Extract table of contents](https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents)
* [Extract text by table of contents item](https://docs.groupdocs.com/display/parsernet/Extract+text+by+table+of+contents+item)
* [Extract table of contents from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents+from+Microsoft+Office+Word+documents)
* [Extract table of contents from EPUB eBooks](https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents+from+EPUB+eBooks)

### Contoh

Contoh berikut menunjukkan cara mengekstrak daftar isi dari file CHM:

```csharp
// Buat sebuah instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Periksa apakah ekstraksi teks didukung
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }

    // Periksa apakah ekstraksi toc didukung
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
 
    // Dapatkan daftar isi
    IEnumerable<TocItem> toc = parser.GetToc();
    
    // Iterasi pada item
    foreach (TocItem i in toc)
    {
        // Cetak teks Toc
        Console.WriteLine(i.Text);
        // Periksa apakah indeks halaman memiliki nilai
        if (i.PageIndex == null)
        {
            continue;
        }
        // Ekstrak teks halaman
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Lihat Juga

* class [TocItem](../../../groupdocs.parser.data/tocitem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->

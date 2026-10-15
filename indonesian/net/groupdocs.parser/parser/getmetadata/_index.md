---
title: "GetMetadata"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mengekstrak metadata dari dokumen."
type: docs
weight: 140
url: /id/net/groupdocs.parser/parser/getmetadata/
---

## Parser.GetMetadata method

Mengekstrak metadata dari dokumen.

```csharp
public IEnumerable<MetadataItem> GetMetadata()
```

### Nilai Kembali

Koleksi item metadata; `null` jika ekstraksi metadata tidak didukung.

### Catatan

**Learn more:**

* [Extract metadata from documents](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+documents)
* [Extract metadata from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+Word+documents)
* [Extract metadata from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+Excel+spreadsheets)
* [Extract metadata from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+PowerPoint+presentations)
* [Extract metadata from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+PDF+documents)
* [Extract metadata from Emails](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Emails)

### Contoh

Contoh berikut menunjukkan cara mengekstrak metadata dari dokumen:

```csharp
// Buat sebuah instance dari kelas Parser
using(Parser parser = new Parser(filePath))
{
    // Ekstrak metadata dari dokumen
    IEnumerable<MetadataItem> metadata = parser.GetMetadata();
    // Periksa apakah ekstraksi metadata didukung
    if(metadata == null)
    {
        Console.WriteLine("Metatada extraction isn't supported");
    }
 
    // Iterasi atas item metadata
    foreach(MetadataItem item in metadata)
    {
        // Cetak nama dan nilai item
        Console.WriteLine(string.Format("{0}: {1}", item.Name, item.Value));
    }
}
```

### Lihat Juga

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->

---
title: "GetContainer"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mengekstrak objek kontainer dari dokumen untuk bekerja dengan format yang berisi lampiran, arsip ZIP, dll."
type: docs
weight: 80
url: /id/net/groupdocs.parser/parser/getcontainer/
---

## Parser.GetContainer method

Mengekstrak objek kontainer dari dokumen untuk bekerja dengan format yang berisi lampiran, arsip ZIP, dll.

```csharp
public IEnumerable<ContainerItem> GetContainer()
```

### Nilai Kembali

Koleksi item kontainer; `null` jika ekstraksi kontainer tidak didukung.

### Catatan

Untuk memeriksa apakah format mendukung ekstraksi lampiran, lihat [Supported Document Formats](https://docs.groupdocs.com/parser/net/supported-document-formats/) (**Extract Containers and Attachments** column).

**Learn more:**

* [Extract data from attachments and ZIP archives](https://docs.groupdocs.com/display/parsernet/Extract+data+from+attachments+and+ZIP+archives)
* [Iterate through container items](https://docs.groupdocs.com/display/parsernet/Iterate+through+container+items)
* [Extract attachments from PDF portfolios](https://docs.groupdocs.com/display/parsernet/Extract+attachments+from+PDF+portfolios)
* [Extract attachments from Emails](https://docs.groupdocs.com/display/parsernet/Extract+attachments+from+Emails)
* [Extract emails from Outlook Storage](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+Outlook+Storage)
* [Extract text from ZIP archive files](https://docs.groupdocs.com/display/parsernet/Extract+text+from+ZIP+archive+files)

### Contoh

Contoh berikut menunjukkan cara mengekstrak lampiran dari sebuah kontainer:

```csharp
// Buat sebuah instance dari kelas Parser
using(Parser parser = new Parser(filePath))
{
    // Ekstrak lampiran dari kontainer
    IEnumerable<ContainerItem> attachments = parser.GetContainer();
    // Periksa apakah ekstraksi kontainer didukung
    if(attachments == null)
    {
        Console.WriteLine("Container extraction isn't supported");
    }
 
    // Iterasi atas lampiran
    foreach(ContainerItem item in attachments)
    {
        // Cetak nama dan ukuran item
        Console.WriteLine(string.Format("{0}: {1}", item.Name, item.Size));
    }
}
```

### Lihat Juga

* class [ContainerItem](../../../groupdocs.parser.data/containeritem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->

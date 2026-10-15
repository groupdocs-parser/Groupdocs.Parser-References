---
title: "DetectFileType"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mendeteksi tipe file dari item kontainer."
type: docs
weight: 60
url: /id/net/groupdocs.parser.data/containeritem/detectfiletype/
---

## ContainerItem.DetectFileType method

Mendeteksi tipe file dari item kontainer.

```csharp
public FileType DetectFileType(FileTypeDetectionMode detectionMode)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| detectionMode | FileTypeDetectionMode | Mendefinisikan mode deteksi tipe file. |

### Nilai Kembali

Sebuah instance dari kelas [`FileType`](../../../groupdocs.parser.options/filetype); [`Unknown`](../../../groupdocs.parser.options/filetype/unknown) jika tipe file tidak terdeteksi.

### Catatan

*detectionMode* parameter provides the ability to control file type detection:

* **Default**. The file type is detected by the file extension; if the file extension isn't recognized, the file type is detected by the file content.
* **Extension**.The file type is detected only by the file extension.
* **Content**. The file type is detected only by the file content.

### Contoh

Contoh berikut menunjukkan cara mendeteksi tipe file dari item kontainer:

```csharp
// Buat sebuah instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Ekstrak lampiran dari kontainer
    IEnumerable<ContainerItem> attachments = parser.GetContainer();
    // Periksa apakah ekstraksi kontainer didukung
    if (attachments == null)
    {
        Console.WriteLine("Container extraction isn't supported");
    }
    // Iterasi atas lampiran
    foreach (ContainerItem item in attachments)
    {
        // Deteksi tipe file
        Options.FileType fileType = item.DetectFileType(Options.FileTypeDetectionMode.Default);

        // Cetak nama dan tipe file
        Console.WriteLine(string.Format("{0}: {1}", item.Name, fileType));
    }
}
```

### Lihat Juga

* class [FileType](../../../groupdocs.parser.options/filetype)
* enum [FileTypeDetectionMode](../../../groupdocs.parser.options/filetypedetectionmode)
* class [ContainerItem](../../containeritem)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->

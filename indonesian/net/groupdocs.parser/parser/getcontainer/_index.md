---
title: GetContainer
second_title: GroupDocs.Parser untuk Referensi .NET API
description: Mengekstrak objek penampung dari dokumen untuk bekerja dengan format yang berisi lampiran arsip ZIP dll.
type: docs
weight: 60
url: /id/net/groupdocs.parser/parser/getcontainer/
---
## Parser.GetContainer method

Mengekstrak objek penampung dari dokumen untuk bekerja dengan format yang berisi lampiran, arsip ZIP, dll.

```csharp
public IEnumerable<ContainerItem> GetContainer()
```

### Nilai Pengembalian

Kumpulan item kontainer; `batal`jika ekstraksi penampung tidak didukung.

### Perkataan

Untuk memeriksa apakah format mendukung ekstraksi lampiran, lihat[Format Dokumen yang Didukung](https://docs.groupdocs.com/parser/net/supported-document-formats/) (**Ekstrak Kontainer dan Lampiran** kolom).

**Belajarlah lagi:**

* [Ekstrak data dari lampiran dan arsip ZIP](https://docs.groupdocs.com/display/parsernet/Extract+data+from+attachments+and+ZIP+archives)
* [Iterasi melalui item kontainer](https://docs.groupdocs.com/display/parsernet/Iterate+through+container+items)
* [Ekstrak lampiran dari portofolio PDF](https://docs.groupdocs.com/display/parsernet/Extract+attachments+from+PDF+portfolios)
* [Ekstrak lampiran dari Email](https://docs.groupdocs.com/display/parsernet/Extract+attachments+from+Emails)
* [Ekstrak email dari Penyimpanan Outlook](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+Outlook+Storage)
* [Ekstrak teks dari file arsip ZIP](https://docs.groupdocs.com/display/parsernet/Extract+text+from+ZIP+archive+files)

### Contoh

Contoh berikut menunjukkan cara mengekstrak lampiran dari wadah:

```csharp
// Buat instance dari kelas Parser
using(Parser parser = new Parser(filePath))
{
    // Ekstrak lampiran dari wadah
    IEnumerable<ContainerItem> attachments = parser.GetContainer();
    // Periksa apakah ekstraksi kontainer didukung
    if(attachments == null)
    {
        Console.WriteLine("Container extraction isn't supported");
    }
 
    // Ulangi lampiran
    foreach(ContainerItem item in attachments)
    {
        // Cetak nama dan ukuran item
        Console.WriteLine(string.Format("{0}: {1}", item.Name, item.Size));
    }
}
```

### Lihat juga

* class [ContainerItem](../../../groupdocs.parser.data/containeritem)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

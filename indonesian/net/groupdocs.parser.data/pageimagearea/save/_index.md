---
title: "Simpan"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menyimpan gambar ke file."
type: docs
weight: 50
url: /id/net/groupdocs.parser.data/pageimagearea/save/
---

## Save(string) {#save}

Menyimpan gambar ke file.

```csharp
public void Save(string filePath)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| filePath | String | Jalur ke file. |

### Contoh

Contoh berikut menunjukkan cara menyimpan gambar ke file:

```csharp
// Buat sebuah instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Ekstrak gambar dari dokumen
    IEnumerable<PageImageArea> images = parser.GetImages();
    
    // Periksa apakah ekstraksi gambar didukung
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }

    // Iterasi melalui gambar
    foreach (PageImageArea image in images)
    {
        // Simpan gambar ke file
        image.Save(Guid.NewGuid().ToString() + image.FileType.Extension);
    }
}
```

### Lihat Juga

* class [PageImageArea](../../pageimagearea)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

---

## Save(string, ImageOptions) {#save_1}

Menyimpan gambar ke file dalam format yang berbeda.

```csharp
public void Save(string filePath, ImageOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| filePath | String | Jalur ke file. |
| options | ImageOptions | Opsi yang digunakan untuk menyimpan gambar. |

### Contoh

Contoh berikut menunjukkan cara menyimpan gambar ke file dalam format yang berbeda:

```csharp
// Buat sebuah instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Ekstrak gambar dari dokumen
    IEnumerable<PageImageArea> images = parser.GetImages();
    
    // Periksa apakah ekstraksi gambar didukung
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }

    // Buat opsi untuk menyimpan gambar dalam format PNG
    ImageOptions options = new ImageOptions(ImageFormat.Png);
    
    // Iterasi melalui gambar
    foreach (PageImageArea image in images)
    {
        // Simpan gambar ke file png
        image.Save(Guid.NewGuid().ToString() + ".png", options);
    }
}
```

### Lihat Juga

* class [ImageOptions](../../../groupdocs.parser.options/imageoptions)
* class [PageImageArea](../../pageimagearea)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->

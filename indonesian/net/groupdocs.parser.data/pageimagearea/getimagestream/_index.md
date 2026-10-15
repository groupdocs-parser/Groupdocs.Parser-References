---
title: "GetImageStream"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mengembalikan aliran gambar."
type: docs
weight: 40
url: /id/net/groupdocs.parser.data/pageimagearea/getimagestream/
---

## GetImageStream() {#getimagestream}

Mengembalikan aliran gambar.

```csharp
public Stream GetImageStream()
```

### Nilai Kembali

Aliran yang berisi gambar.

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
        // Buka aliran gambar
        using (Stream imageStream = image.GetImageStream())
        {
            // Buat file untuk menyimpan gambar
            using (Stream destStream = File.Create(Guid.NewGuid().ToString() + image.FileType.Extension))
            {
                byte[] buffer = new byte[4096];
                int readed = 0;

                do
                {
                    // Baca data dari aliran gambar
                    readed = imageStream.Read(buffer, 0, buffer.Length);

                    if (readed > 0)
                    {
                        // Tulis data ke aliran file
                        destStream.Write(buffer, 0, readed);
                    }
                }
                while (readed > 0);
            }
        }
    }
}
```

### Lihat Juga

* class [PageImageArea](../../pageimagearea)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

---

## GetImageStream(ImageOptions) {#getimagestream_1}

Mengembalikan aliran gambar dalam format yang berbeda.

```csharp
public Stream GetImageStream(ImageOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| options | ImageOptions | Opsi yang digunakan untuk mengekstrak gambar. |

### Nilai Kembali

Aliran yang berisi gambar.

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
        // Buka aliran gambar
        using (Stream imageStream = image.GetImageStream(options))
        {
            // Buat file untuk menyimpan gambar
            using (Stream destStream = File.Create(Guid.NewGuid().ToString() + ".png"))
            {
                byte[] buffer = new byte[4096];
                int readed = 0;

                do
                {
                    // Baca data dari aliran gambar
                    readed = imageStream.Read(buffer, 0, buffer.Length);

                    if (readed > 0)
                    {
                        // Tulis data ke aliran file
                        destStream.Write(buffer, 0, readed);
                    }
                }
                while (readed > 0);
            }
        }
    }
}
```

### Lihat Juga

* class [ImageOptions](../../../groupdocs.parser.options/imageoptions)
* class [PageImageArea](../../pageimagearea)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->

---
title: GetImageStream
second_title: .NET API Başvurusu için GroupDocs.Parser
description: Görüntü akışını döndürür.
type: docs
weight: 40
url: /tr/net/groupdocs.parser.data/pageimagearea/getimagestream/
---
## GetImageStream() {#getimagestream}

Görüntü akışını döndürür.

```csharp
public Stream GetImageStream()
```

### Geri dönüş değeri

Görüntü içeren bir akış.

### Örnekler

Aşağıdaki örnek, görüntülerin dosyalara nasıl kaydedileceğini gösterir:

```csharp
// Parser sınıfının bir örneğini oluşturun
using (Parser parser = new Parser(filePath))
{
    // Belgeden görüntüleri ayıklayın
    IEnumerable<PageImageArea> images = parser.GetImages();
    
    // Görüntü çıkarmanın desteklenip desteklenmediğini kontrol edin
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }

    // Görüntüler üzerinde yineleme
    foreach (PageImageArea image in images)
    {
        // Görüntü akışını aç
        using (Stream imageStream = image.GetImageStream())
        {
            // Görüntüyü kaydetmek için dosyayı oluşturun
            using (Stream destStream = File.Create(Guid.NewGuid().ToString() + image.FileType.Extension))
            {
                byte[] buffer = new byte[4096];
                int readed = 0;

                do
                {
                    // Görüntü akışındaki verileri oku
                    readed = imageStream.Read(buffer, 0, buffer.Length);

                    if (readed > 0)
                    {
                        // Dosya akışına veri yaz
                        destStream.Write(buffer, 0, readed);
                    }
                }
                while (readed > 0);
            }
        }
    }
}
```

### Ayrıca bakınız

* class [PageImageArea](../../pageimagearea)
* ad alanı [GroupDocs.Parser.Data](../../pageimagearea)
* toplantı [GroupDocs.Parser](../../../)

---

## GetImageStream(ImageOptions) {#getimagestream_1}

Görüntü akışını farklı bir biçimde döndürür.

```csharp
public Stream GetImageStream(ImageOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| options | ImageOptions | Görüntüyü çıkarmak için kullanılan seçenekler. |

### Geri dönüş değeri

Görüntü içeren bir akış.

### Örnekler

Aşağıdaki örnek, görüntülerin farklı bir biçimde dosyalara nasıl kaydedileceğini gösterir:

```csharp
// Parser sınıfının bir örneğini oluşturun
using (Parser parser = new Parser(filePath))
{
    // Belgeden görüntüleri ayıklayın
    IEnumerable<PageImageArea> images = parser.GetImages();
    
    // Görüntü çıkarmanın desteklenip desteklenmediğini kontrol edin
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }

    // Resimleri PNG formatında kaydetmek için seçenekler oluşturun
    ImageOptions options = new ImageOptions(ImageFormat.Png);
    
    // Görüntüler üzerinde yineleme
    foreach (PageImageArea image in images)
    {
        // Görüntü akışını aç
        using (Stream imageStream = image.GetImageStream(options))
        {
            // Görüntüyü kaydetmek için dosyayı oluşturun
            using (Stream destStream = File.Create(Guid.NewGuid().ToString() + ".png"))
            {
                byte[] buffer = new byte[4096];
                int readed = 0;

                do
                {
                    // Görüntü akışındaki verileri oku
                    readed = imageStream.Read(buffer, 0, buffer.Length);

                    if (readed > 0)
                    {
                        // Dosya akışına veri yaz
                        destStream.Write(buffer, 0, readed);
                    }
                }
                while (readed > 0);
            }
        }
    }
}
```

### Ayrıca bakınız

* class [ImageOptions](../../../groupdocs.parser.options/imageoptions)
* class [PageImageArea](../../pageimagearea)
* ad alanı [GroupDocs.Parser.Data](../../pageimagearea)
* toplantı [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
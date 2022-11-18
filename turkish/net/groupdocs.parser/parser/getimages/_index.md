---
title: GetImages
second_title: .NET API Başvurusu için GroupDocs.Parser
description: Belgeden görüntüleri ayıklar.
type: docs
weight: 110
url: /tr/net/groupdocs.parser/parser/getimages/
---
## GetImages() {#getimages}

Belgeden görüntüleri ayıklar.

```csharp
public IEnumerable<PageImageArea> GetImages()
```

### Geri dönüş değeri

Koleksiyonu[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) nesneler; `hükümsüz` resim çıkarma desteklenmiyorsa.

### Notlar

**Daha fazla bilgi edin:**

* [Belgelerden görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Görüntüleri dosyalara çıkarın](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Microsoft Office Word belgelerinden görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Microsoft Office Excel elektronik tablolarından görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Microsoft Office PowerPoint sunumlarından görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [E-postalardan görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [PDF belgelerinden görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Örnekler

Aşağıdaki örnek, tüm görüntülerin tüm belgeden nasıl çıkarılacağını gösterir:

```csharp
// Parser sınıfının bir örneğini oluşturun
using (Parser parser = new Parser(filePath))
{
    // görüntüleri ayıklayın
    IEnumerable<PageImageArea> images = parser.GetImages();
    // Görüntü çıkarmanın desteklenip desteklenmediğini kontrol edin
    if (images == null)
    {
        Console.WriteLine("Images extraction isn't supported");
        return;
    }
    // Görüntüler üzerinde yineleme
    foreach (PageImageArea image in images)
    {
        // Bir sayfa dizini, dikdörtgen ve görüntü türü yazdırın:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Ayrıca bakınız

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

---

## GetImages(PageAreaOptions) {#getimages_1}

(görüntüleri içeren dikdörtgen alanı ayarlamak için) özelleştirme seçeneklerini kullanarak görüntüleri belgeden çıkarır.

```csharp
public IEnumerable<PageImageArea> GetImages(PageAreaOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| options | PageAreaOptions | Görüntü çıkarma seçenekleri. |

### Geri dönüş değeri

Koleksiyonu[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) nesneler; `hükümsüz` resim çıkarma desteklenmiyorsa.

### Notlar

**Daha fazla bilgi edin:**

* [Belgelerden görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Görüntüleri dosyalara çıkarın](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Belge sayfası alanından görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Microsoft Office Word belgelerinden görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Microsoft Office Excel elektronik tablolarından görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Microsoft Office PowerPoint sunumlarından görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [E-postalardan görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [PDF belgelerinden görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Örnekler

Aşağıdaki örnek, yalnızca sol üst köşeden görüntülerin nasıl çıkarılacağını gösterir:

```csharp
// Parser sınıfının bir örneğini oluşturun
using (Parser parser = new Parser(filePath))
{
    // Görüntü çıkarma için kullanılan seçenekleri oluşturun
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(0, 0), new Size(300, 100)));
    // Bir sayfanın sol üst köşesindeki görüntüleri çıkarın:
    IEnumerable<PageImageArea> images = parser.GetImages(options);
    // Görüntü çıkarmanın desteklenip desteklenmediğini kontrol edin
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }
    // Görüntüler üzerinde yineleme
    foreach (PageImageArea image in images)
    {
        // Bir sayfa dizini, dikdörtgen ve görüntü türü yazdırın:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Ayrıca bakınız

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

---

## GetImages(int) {#getimages_2}

Belge sayfasından görüntüleri ayıklar.

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pageIndex | Int32 | Sıfır tabanlı sayfa dizini. |

### Geri dönüş değeri

Koleksiyonu[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) nesneler; `hükümsüz` resim çıkarma desteklenmiyorsa.

### Notlar

**Daha fazla bilgi edin:**

* [Belgelerden görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Görüntüleri dosyalara çıkarın](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Belge sayfasından görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Microsoft Office Word belgelerinden görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Microsoft Office Excel elektronik tablolarından görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Microsoft Office PowerPoint sunumlarından görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [E-postalardan görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [PDF belgelerinden görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Örnekler

Bir belge sayfasından görüntüleri çıkarmak için aşağıdaki yöntem kullanılır:

```csharp
// Parser sınıfının bir örneğini oluşturun
using (Parser parser = new Parser(filePath))
{
    // Belgenin resim çıkarmayı destekleyip desteklemediğini kontrol edin
    if (!parser.Features.Images)
    {
        Console.WriteLine("Document isn't supports images extraction.");
        return;
    }
    
    // Belge bilgilerini al
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Belgenin sayfaları olup olmadığını kontrol edin
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // Sayfalar üzerinde yinele
    for (int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Bir sayfa numarası yazdır 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Görüntüler üzerinde yineleme
        // Görüntü çıkarma özelliği desteğini daha önce kontrol ettiğimiz için boş denetimi yok sayıyoruz
        foreach (PageImageArea image in parser.GetImages(pageIndex))
        {
            // Bir dikdörtgen ve görüntü türü yazdır
            Console.WriteLine(string.Format("R: {0}, Text: {1}", image.Rectangle, image.FileType));
        }
    }
}
```

### Ayrıca bakınız

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

---

## GetImages(int, PageAreaOptions) {#getimages_3}

Özelleştirme seçeneklerini kullanarak belge sayfasından görüntüleri çıkarır (resimleri içeren dikdörtgen alanı ayarlamak için).

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex, PageAreaOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pageIndex | Int32 | Sıfır tabanlı sayfa dizini. |
| options | PageAreaOptions | Görüntü çıkarma seçenekleri. |

### Geri dönüş değeri

Koleksiyonu[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) nesneler; `hükümsüz` resim çıkarma desteklenmiyorsa.

### Notlar

**Daha fazla bilgi edin:**

* [Belgelerden görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Görüntüleri dosyalara çıkarın](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Belge sayfasından görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Belge sayfası alanından görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Microsoft Office Word belgelerinden görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Microsoft Office Excel elektronik tablolarından görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Microsoft Office PowerPoint sunumlarından görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [E-postalardan görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [PDF belgelerinden görüntüleri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Ayrıca bakınız

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

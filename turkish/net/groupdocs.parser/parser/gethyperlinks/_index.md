---
title: GetHyperlinks
second_title: .NET API Başvurusu için GroupDocs.Parser
description: Belgeden köprüleri çıkarır.
type: docs
weight: 100
url: /tr/net/groupdocs.parser/parser/gethyperlinks/
---
## GetHyperlinks() {#gethyperlinks}

Belgeden köprüleri çıkarır.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks()
```

### Geri dönüş değeri

Koleksiyonu[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) nesneler; `hükümsüz` köprü çıkarma desteklenmiyorsa.

### Örnekler

Aşağıdaki örnek, tüm köprülerin tüm belgeden nasıl çıkarılacağını gösterir:

```csharp
// Parser sınıfının bir örneğini oluşturun
using (Parser parser = new Parser(filePath))
{
    // Belgenin hiper bağlantı çıkarmayı destekleyip desteklemediğini kontrol edin
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Belgeden köprüleri çıkar
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks();
    // Köprüler üzerinde yineleme
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Köprü metnini yazdır
        Console.WriteLine(h.Text);
        // Köprü URL'sini yazdır
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Ayrıca bakınız

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int) {#gethyperlinks_2}

Belge sayfasından köprüleri çıkarır.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pageIndex | Int32 | Sıfır tabanlı sayfa dizini. |

### Geri dönüş değeri

Koleksiyonu[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) nesneler; `hükümsüz` köprü çıkarma desteklenmiyorsa.

### Örnekler

Aşağıdaki örnek, belge sayfasından köprülerin nasıl çıkarılacağını gösterir:

```csharp
// Parser sınıfının bir örneğini oluşturun
using (Parser parser = new Parser(filePath))
{
    // Belgenin hiper bağlantı çıkarmayı destekleyip desteklemediğini kontrol edin
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
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
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Bir sayfa numarası yazdır 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Belge sayfasından köprüleri ayıklayın
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex);
        // Köprüler üzerinde yineleme
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Köprü metnini yazdır
            Console.WriteLine(h.Text);
            // Köprü URL'sini yazdır
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
    }
}
```

### Ayrıca bakınız

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

---

## GetHyperlinks(PageAreaOptions) {#gethyperlinks_1}

Özelleştirme seçeneklerini kullanarak belgeden köprüleri çıkarır (köprüleri içeren dikdörtgen alanı ayarlamak için).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(PageAreaOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| options | PageAreaOptions | Köprü çıkarma seçenekleri. |

### Geri dönüş değeri

Koleksiyonu[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) nesneler; `hükümsüz` köprü çıkarma desteklenmiyorsa.

### Örnekler

Aşağıdaki örnek, belge sayfası alanından köprülerin nasıl çıkarılacağını gösterir:

```csharp
// Parser sınıfının bir örneğini oluşturun
using (Parser parser = new Parser(filePath))
{
    // Belgenin hiper bağlantı çıkarmayı destekleyip desteklemediğini kontrol edin
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Köprü çıkarma için kullanılan seçenekleri oluşturun
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Belge sayfası alanından köprüleri ayıklayın
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(options);
    // Köprüler üzerinde yineleme
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Köprü metnini yazdır
        Console.WriteLine(h.Text);
        // Köprü URL'sini yazdır
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Ayrıca bakınız

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int, PageAreaOptions) {#gethyperlinks_3}

Özelleştirme seçeneklerini kullanarak belge sayfasından köprüleri çıkarır (köprüleri içeren dikdörtgen alanı ayarlamak için).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex, PageAreaOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pageIndex | Int32 | Sıfır tabanlı sayfa dizini. |
| options | PageAreaOptions | Köprü çıkarma seçenekleri. |

### Geri dönüş değeri

Koleksiyonu[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) nesneler; `hükümsüz` köprü çıkarma desteklenmiyorsa.

### Örnekler

Aşağıdaki örnek, özelleştirme seçeneklerini kullanarak köprülerin belge sayfası alanından nasıl çıkarılacağını gösterir:

```csharp
// Parser sınıfının bir örneğini oluşturun
using (Parser parser = new Parser(filePath))
{
    // Belgenin hiper bağlantı çıkarmayı destekleyip desteklemediğini kontrol edin
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
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
    
    // Köprü çıkarma için kullanılan seçenekleri oluşturun
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Sayfalar üzerinde yinele
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Bir sayfa numarası yazdır 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));         
        // Belge sayfası alanından köprüleri ayıklayın
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex, options);
        // Köprüler üzerinde yineleme
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Köprü metnini yazdır
            Console.WriteLine(h.Text);
            // Köprü URL'sini yazdır
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
}
```

### Ayrıca bakınız

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

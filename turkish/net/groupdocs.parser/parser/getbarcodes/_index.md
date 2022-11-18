---
title: GetBarcodes
second_title: .NET API Başvurusu için GroupDocs.Parser
description: Belgeden barkodları çıkarır.
type: docs
weight: 50
url: /tr/net/groupdocs.parser/parser/getbarcodes/
---
## GetBarcodes() {#getbarcodes}

Belgeden barkodları çıkarır.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes()
```

### Geri dönüş değeri

Koleksiyonu[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) nesneler; `hükümsüz` barkod çıkarma desteklenmiyorsa.

### Örnekler

Aşağıdaki örnek, bir belgeden barkodların nasıl çıkarılacağını gösterir:

```csharp
// Parser sınıfının bir örneğini oluşturun
using (Parser parser = new Parser(filePath))
{
    // Barkodları belgeden çıkarın.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes();

    // Barkodlar üzerinde yineleme
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Sayfa dizinini yazdır
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Barkod değerini yazdır
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Ayrıca bakınız

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

---

## GetBarcodes(int) {#getbarcodes_2}

Belge sayfasından barkodları çıkarır.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pageIndex | Int32 | Sıfır tabanlı sayfa dizini. |

### Geri dönüş değeri

Koleksiyonu[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) nesneler; `hükümsüz` barkod çıkarma desteklenmiyorsa.

### Örnekler

Aşağıdaki örnek, bir belge sayfasından barkodların nasıl çıkarılacağını gösterir:

```csharp
// Parser sınıfının bir örneğini oluşturun
using (Parser parser = new Parser(filePath))
{
    // İkinci belge sayfasından barkodları çıkarın.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(1);

    // Barkodlar üzerinde yineleme
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Sayfa dizinini yazdır
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Barkod değerini yazdır
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Ayrıca bakınız

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

---

## GetBarcodes(PageAreaOptions) {#getbarcodes_1}

Özelleştirme seçeneklerini kullanarak belgeden barkodları çıkarır (barkodları içeren dikdörtgen alanı ayarlamak için).

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(PageAreaOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| options | PageAreaOptions | Barkod çıkarma seçenekleri. |

### Geri dönüş değeri

Koleksiyonu[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) nesneler; `hükümsüz` barkod çıkarma desteklenmiyorsa.

### Örnekler

Aşağıdaki örnek, barkodların sağ üst köşeden nasıl çıkarılacağını gösterir.

```csharp
// Parser sınıfının bir örneğini oluşturun
using (Parser parser = new Parser(filePath))
{
    // Barkod çıkarma için kullanılan seçenekleri oluşturun
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(590, 80), new Size(150, 150)));
    // Barkodları sağ üst köşeden çıkarın.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(options);

    // Barkodlar üzerinde yineleme
    foreach (PageBarcodeArea barcode in barcodes)
    {
        // Sayfa dizinini yazdır
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Barkod değerini yazdır
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Ayrıca bakınız

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

---

## GetBarcodes(int, PageAreaOptions) {#getbarcodes_3}

Özelleştirme seçeneklerini kullanarak belge sayfasından barkodları çıkarır (barkodları içeren dikdörtgen alanı ayarlamak için).

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex, PageAreaOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pageIndex | Int32 | Sıfır tabanlı sayfa dizini. |
| options | PageAreaOptions | Barkod çıkarma seçenekleri. |

### Geri dönüş değeri

Koleksiyonu[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) nesneler; `hükümsüz` barkod çıkarma desteklenmiyorsa.

### Ayrıca bakınız

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

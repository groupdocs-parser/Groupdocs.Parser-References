---
title: MoveTo
second_title: .NET API Başvurusu için GroupDocs.Parser
description: Aynı boyut ayırıcılar ve konum ile yeni bir düzen oluşturur.point .
type: docs
weight: 50
url: /tr/net/groupdocs.parser.templates/templatetablelayout/moveto/
---
## TemplateTableLayout.MoveTo method

Aynı boyut, ayırıcılar ve konum ile yeni bir düzen oluşturur.*point* .

```csharp
public TemplateTableLayout MoveTo(Point point)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| point | Point | Yeni düzenin konumu. |

### Geri dönüş değeri

Aynı boyuta, ayırıcılara ve konuma sahip yeni bir düzen*point*.

### Örnekler

Bu işlevsellik Tablo Düzenini taşımaya izin verir.

Örneğin, bir belgenin her sayfasında tablolar bulunur (veya sayfada tablosu olan bir dizi belge). Bu tablolar, konuma ve içeriğe göre farklılık gösterir, ancak aynı sütunlara ve satırlara sahiptir. Bu durumda bir kullanıcı tanımlayabilir[`TemplateTableLayout`](../../templatetablelayout) itiraz etmek`(0, 0)` bir kez ve ardından kesin tablonun konumuna taşıyın.

Tablo konumu sayfanın diğer nesnesine bağlıysa, kullanıcı tanımlayabilir[`TemplateTableLayout`](../../templatetablelayout) şablon belgesinde nesne tabanlı ve ardından onu bir bağlantı nesnesine göre taşıyın. Örneğin, bu bir özet tablosuysa ve ise, bunu ayrıntılar tablosu izler (farklı sayıda satır içerebilir). Bu durumda bir kullanıcı tanımlayabilir[`TemplateTableLayout`](../../templatetablelayout)şablon belgesindeki nesneyi (bilinen ayrıntılar tablosu dikdörtgeni ile) ve ardından öğesini taşıyın[`TemplateTableLayout`](../../templatetablelayout) şablon ve gerçek belgenin ayrıntı tablosu dikdörtgeni arasındaki farka göre nesne.

`MoveTo` method geçerli nesnenin bir kopyasını döndürür. Bir kullanıcı herhangi bir koordinatı iletebilir (negatif bile - bu durumda düzen sola/üste taşınacaktır).

```csharp
// Bir tablo düzeni oluştur
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 0, 25, 150, 180, 230 },
    new double[] { 0, 15, 30, 45, 60, 75 });

// Bir dikdörtgen yazdır
Rectangle rect = layout.Rectangle;

// Yazdırır: konum: (0, 0) boyut: (230, 75)
Console.WriteLine(string.Format("pos: ({0}, {1}) size: ({2}, {3})", rect.Left, rect.Top, rect.Size.Width, rect.Size.Height));

// Düzeni belirli tablo konumuna taşı
TemplateTableLayout movedLayout = layout.MoveTo(new Point(315, 250));

// İlk ayırıcıların taşındığından emin olun:
Console.WriteLine(movedLayout.VerticalSeparators[0]); // yazdırır: 315
Console.WriteLine(movedLayout.HorizontalSeparators[0]); // yazdırır: 250

Rectangle movedRect = movedLayout.Rectangle;

// Baskılar: konum: (315, 250) boyut: (230, 75)
Console.WriteLine(string.Format("pos: ({0}, {1}) size: ({2}, {3})", movedRect.Left, movedRect.Top, movedRect.Size.Width, movedRect.Size.Height));

// moveLayout nesnesi, layout nesnesinin bir kopyasıdır, dolayısıyla ayırıcıları, orijinal layout üzerinde bir etkisi olmadan ayarlayabiliriz:
movedLayout.HorizontalSeparators.Add(90);

Console.WriteLine(movedLayout.HorizontalSeparators.Count); // yazdırır: 7
Console.WriteLine(layout.HorizontalSeparators.Count); // yazdırır: 6
```

### Ayrıca bakınız

* class [Point](../../../groupdocs.parser.data/point)
* class [TemplateTableLayout](../../templatetablelayout)
* ad alanı [GroupDocs.Parser.Templates](../../templatetablelayout)
* toplantı [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

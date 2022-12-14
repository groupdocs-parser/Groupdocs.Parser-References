---
title: Item
second_title: .NET API Başvurusu için GroupDocs.Parser
description: Alan verilerini bir dizine göre alır.
type: docs
weight: 30
url: /tr/net/groupdocs.parser.data/documentdata/item/
---
## DocumentData indexer

Alan verilerini bir dizine göre alır.

```csharp
public FieldData this[int index] { get; }
```

| Parametre | Tanım |
| --- | --- |
| index | Alanın sıfır tabanlı dizini. |

### Geri dönüş değeri

bir örneği[`FieldData`](../../fielddata) sınıf.

### Örnekler

Tüm alanlar aracılığıyla yineleme:

[`FieldData`](../../fielddata) sınıf alan verilerini temsil eder. alana bağlı olarak[`PageArea`](../../fielddata/pagearea) property , mirasçılarından herhangi birini içerebilir[`PageArea`](../../pagearea) sınıf. Örneğin,[`ParseForm`](../../../groupdocs.parser/parser/parseform) method yalnızca metin alanlarını çıkarır:

```csharp
for (int i = 0; i < data.Count; i++)
{
    Console.Write(data[i].Name + ": ");
    PageTextArea area = data[i].PageArea as PageTextArea;
    Console.WriteLine(area == null ? "Not a template field" : area.Text);
}
```

```csharp
// Ayrıştırıcıyı oluştur
using (Parser parser = new Parser(filePath))
{
    // PDF Formundan verileri ayıklayın
    DocumentData data = parser.ParseForm();
    // Ayıklanan alanlar üzerinde yineleme yapın
    for (int i = 0; i < data.Count; i++)
    {
        // Ayıklanan alanı al
        FieldData field = data[i];
        // alan adını yazdır
        Console.Write(field.Name + ": ");
        // Alan değerinin bir metin olup olmadığını kontrol edin ve yazdırın
        PageTextArea area = field.PageArea as PageTextArea;
        Console.WriteLine(area == null ? "Not a template field" : area.Text);
    }
}
```

### Ayrıca bakınız

* class [FieldData](../../fielddata)
* class [DocumentData](../../documentdata)
* ad alanı [GroupDocs.Parser.Data](../../documentdata)
* toplantı [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

---
title: PageArea
second_title: .NET API Başvurusu için GroupDocs.Parser
description: Alanın değerini alır.
type: docs
weight: 40
url: /tr/net/groupdocs.parser.data/fielddata/pagearea/
---
## FieldData.PageArea property

Alanın değerini alır.

```csharp
public PageArea PageArea { get; }
```

### Mülk değeri

bir örneği[`PageArea`](../../pagearea) alanın değerini temsil eden sınıf.

### Örnekler

Alana bağlı olarak`PageArea` property , mirasçılarından herhangi birini içerebilir[`PageArea`](../../pagearea) sınıf. Örneğin,[`ParseForm`](../../../groupdocs.parser/parser/parseform) yöntem yalnızca metin alanlarını ayıklar.

```csharp
// alan verilerini al
FieldData field = data[i];
// Alan verilerinin bir metin içerip içermediğini kontrol edin
if(field.PageArea is PageTextArea)
{
    // Alan metin değerini yazdır
    Console.WriteLine(field.Text);
}
```

### Ayrıca bakınız

* class [PageArea](../../pagearea)
* class [FieldData](../../fielddata)
* ad alanı [GroupDocs.Parser.Data](../../fielddata)
* toplantı [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
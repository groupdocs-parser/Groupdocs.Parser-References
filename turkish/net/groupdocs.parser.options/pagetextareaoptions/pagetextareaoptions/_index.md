---
title: PageTextAreaOptions
second_title: .NET API Başvurusu için GroupDocs.Parser
description: Yeni bir örneğini başlatır.PageTextAreaOptionsgroupdocs.parser.options/pagetextareaoptions düzenli ifade ile sınıf. Diğer seçenekler varsayılan olarak ayarlanmıştır ayrıntılar için açıklamalara bakın.
type: docs
weight: 10
url: /tr/net/groupdocs.parser.options/pagetextareaoptions/pagetextareaoptions/
---
## PageTextAreaOptions(string) {#constructor}

Yeni bir örneğini başlatır.[`PageTextAreaOptions`](../../pagetextareaoptions) düzenli ifade ile sınıf. Diğer seçenekler varsayılan olarak ayarlanmıştır (ayrıntılar için açıklamalara bakın).

```csharp
public PageTextAreaOptions(string expression)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| expression | String | Normal ifade. |

### Notlar

Aşağıdaki özellikler varsayılan değerlere sahiptir:

**[`MatchCase`](../matchcase)**

`yanlış`

**[`UniteSegments`](../unitesegments)**

`yanlış`

**[`IgnoreFormatting`](../ignoreformatting)**

`yanlış`

**[`Rectangle`](../../pageareaoptions/rectangle)**

`hükümsüz`

### Ayrıca bakınız

* class [PageTextAreaOptions](../../pagetextareaoptions)
* ad alanı [GroupDocs.Parser.Options](../../pagetextareaoptions)
* toplantı [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle) {#constructor_2}

Yeni bir örneğini başlatır.[`PageTextAreaOptions`](../../pagetextareaoptions) düzenli ifade ve dikdörtgen alan ile class . Diğer seçenekler varsayılan olarak ayarlanmıştır (ayrıntılar için açıklamalara bakın).

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| expression | String | Normal ifade. |
| rectangle | Rectangle | Sayfa alanlarını içeren dikdörtgen alan. |

### Notlar

Aşağıdaki özellikler varsayılan değerlere sahiptir:

**[`MatchCase`](../matchcase)**

`yanlış`

**[`UniteSegments`](../unitesegments)**

`yanlış`

**[`IgnoreFormatting`](../ignoreformatting)**

`yanlış`

### Ayrıca bakınız

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* ad alanı [GroupDocs.Parser.Options](../../pagetextareaoptions)
* toplantı [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle) {#constructor_1}

Yeni bir örneğini başlatır.[`PageTextAreaOptions`](../../pagetextareaoptions) sınıf.

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| expression | String | Normal ifade. |
| matchCase | Boolean | Bir metin büyük/küçük harfin yoksayılmayacağını gösteren değer. |
| uniteSegments | Boolean | Segmentlerin birleştirilip birleştirilmediğini gösteren değer. |
| ignoreFormatting | Boolean | Metin biçimlendirmesinin göz ardı edilip edilmediğini gösteren değer. |
| rectangle | Rectangle | Sayfa alanlarını içeren dikdörtgen alan. |

### Ayrıca bakınız

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* ad alanı [GroupDocs.Parser.Options](../../pagetextareaoptions)
* toplantı [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
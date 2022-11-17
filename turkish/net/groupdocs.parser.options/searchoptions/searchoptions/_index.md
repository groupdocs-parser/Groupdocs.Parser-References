---
title: SearchOptions
second_title: .NET API Başvurusu için GroupDocs.Parser
description: Yeni bir örneğini başlatır.SearchOptionsgroupdocs.parser.options/searchoptions sınıf.
type: docs
weight: 10
url: /tr/net/groupdocs.parser.options/searchoptions/searchoptions/
---
## SearchOptions(bool, bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_3}

Yeni bir örneğini başlatır.[`SearchOptions`](../../searchoptions) sınıf.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages, HighlightOptions leftHighlightOptions, 
    HighlightOptions rightHighlightOptions)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| matchCase | Boolean | Bir metin büyük/küçük harfin yoksayılmayacağını gösteren değer. |
| matchWholeWord | Boolean | Metin aramanın tam bir sözcükle sınırlı olup olmadığını gösteren değer. |
| useRegularExpression | Boolean | Normal bir ifadenin kullanılıp kullanılmadığını gösteren değer. |
| searchByPages | Boolean | Aramanın sayfalara göre yapılıp yapılmadığını gösteren değer. |
| leftHighlightOptions | HighlightOptions | Sol vurgu için seçenekler. |
| rightHighlightOptions | HighlightOptions | Sağ vurgu için seçenekler. |

### Ayrıca bakınız

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* ad alanı [GroupDocs.Parser.Options](../../searchoptions)
* toplantı [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_5}

Yeni bir örneğini başlatır.[`SearchOptions`](../../searchoptions) sol ve sağ vurgu çıkarma için vurgulama seçenekleriyle öğesini aramak için kullanılan sınıf.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| matchCase | Boolean | Bir metin büyük/küçük harfin yoksayılmayacağını gösteren değer. |
| matchWholeWord | Boolean | Metin aramanın tam bir sözcükle sınırlı olup olmadığını gösteren değer. |
| useRegularExpression | Boolean | Normal bir ifadenin kullanılıp kullanılmadığını gösteren değer. |
| leftHighlightOptions | HighlightOptions | Sol vurgu için seçenekler. |
| rightHighlightOptions | HighlightOptions | Sağ vurgu için seçenekler. |

### Ayrıca bakınız

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* ad alanı [GroupDocs.Parser.Options](../../searchoptions)
* toplantı [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions) {#constructor_4}

Yeni bir örneğini başlatır.[`SearchOptions`](../../searchoptions) sol ve sağ vurgu çıkarma için aynı vurgulama seçenekleri ile search için kullanılan sınıf.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions highlightOptions)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| matchCase | Boolean | Bir metin büyük/küçük harfin yoksayılmayacağını gösteren değer. |
| matchWholeWord | Boolean | Metin aramanın tam bir sözcükle sınırlı olup olmadığını gösteren değer. |
| useRegularExpression | Boolean | Normal bir ifadenin kullanılıp kullanılmadığını gösteren değer. |
| highlightOptions | HighlightOptions | Her iki vurgu için seçenekler. |

### Ayrıca bakınız

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* ad alanı [GroupDocs.Parser.Options](../../searchoptions)
* toplantı [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool) {#constructor_1}

Yeni bir örneğini başlatır.[`SearchOptions`](../../searchoptions) vurgu çıkarma olmadan aramak için kullanılan sınıf.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| matchCase | Boolean | Bir metin büyük/küçük harfin yoksayılmayacağını gösteren değer. |
| matchWholeWord | Boolean | Metin aramanın tam bir sözcükle sınırlı olup olmadığını gösteren değer. |
| useRegularExpression | Boolean | Normal bir ifadenin kullanılıp kullanılmadığını gösteren değer. |

### Ayrıca bakınız

* class [SearchOptions](../../searchoptions)
* ad alanı [GroupDocs.Parser.Options](../../searchoptions)
* toplantı [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, bool) {#constructor_2}

Yeni bir örneğini başlatır.[`SearchOptions`](../../searchoptions) vurgu çıkarma olmadan and sayfalarına göre arama yapmak için kullanılan sınıf.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| matchCase | Boolean | Bir metin büyük/küçük harfin yoksayılmayacağını gösteren değer. |
| matchWholeWord | Boolean | Metin aramanın tam bir sözcükle sınırlı olup olmadığını gösteren değer. |
| useRegularExpression | Boolean | Normal bir ifadenin kullanılıp kullanılmadığını gösteren değer. |
| searchByPages | Boolean | Aramanın sayfalara göre yapılıp yapılmadığını gösteren değer. |

### Ayrıca bakınız

* class [SearchOptions](../../searchoptions)
* ad alanı [GroupDocs.Parser.Options](../../searchoptions)
* toplantı [GroupDocs.Parser](../../../)

---

## SearchOptions() {#constructor}

Yeni bir örneğini başlatır.[`SearchOptions`](../../searchoptions) varsayılan değerlere sahip sınıf. Ayrıntılar için açıklamalara bakın.

```csharp
public SearchOptions()
```

### Notlar

Aşağıdaki özellikler varsayılan değerlere sahiptir:

**[`MatchCase`](../matchcase)**

`yanlış`

**[`MatchWholeWord`](../matchwholeword)**

`yanlış`

**[`UseRegularExpression`](../useregularexpression)**

`yanlış`

**[`LeftHighlightOptions`](../lefthighlightoptions)**

`hükümsüz`

**[`RightHighlightOptions`](../righthighlightoptions)**

`hükümsüz`

### Ayrıca bakınız

* class [SearchOptions](../../searchoptions)
* ad alanı [GroupDocs.Parser.Options](../../searchoptions)
* toplantı [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

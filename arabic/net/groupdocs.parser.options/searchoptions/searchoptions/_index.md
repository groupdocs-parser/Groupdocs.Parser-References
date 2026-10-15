---
title: "SearchOptions"
second_title: "GroupDocs.Parser لـ .NET API مرجع"
description: "ينشئ مثالا جديدا للفئة SearchOptionsgroupdocs.parser.options/searchoptions."
type: docs
weight: 10
url: /ar/net/groupdocs.parser.options/searchoptions/searchoptions/
---

## SearchOptions(bool, bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_3}

ينشئ مثالا جديدا للفئة [`SearchOptions`](../../searchoptions).

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages, HighlightOptions leftHighlightOptions, 
    HighlightOptions rightHighlightOptions)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| matchCase | Boolean | القيمة التي تشير إلى ما إذا كان تمييز حالة النص غير متجاهل. |
| matchWholeWord | Boolean | القيمة التي تشير إلى ما إذا كان البحث النصي يقتصر على كلمة كاملة. |
| useRegularExpression | Boolean | القيمة التي تشير إلى ما إذا تم استخدام تعبير نمطي. |
| searchByPages | Boolean | القيمة التي تشير إلى ما إذا تم إجراء البحث حسب الصفحات. |
| leftHighlightOptions | HighlightOptions | الخيارات لتسليط الضوء الأيسر. |
| rightHighlightOptions | HighlightOptions | الخيارات لتسليط الضوء الأيمن. |

### انظر أيضًا

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, int, HighlightOptions, HighlightOptions) {#constructor_6}

ينشئ مثيلاً جديدًا من الفئة [`SearchOptions`](../../searchoptions) مع حد الصفحات.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| matchCase | Boolean | القيمة التي تشير إلى ما إذا كان تمييز حالة النص غير متجاهل. |
| matchWholeWord | Boolean | القيمة التي تشير إلى ما إذا كان البحث النصي يقتصر على كلمة كاملة. |
| useRegularExpression | Boolean | القيمة التي تشير إلى ما إذا تم استخدام تعبير نمطي. |
| maxPageIndex | Int32 | القيمة التي تشير إلى ما إذا كان البحث يتم حسب الصفحات. |
| leftHighlightOptions | HighlightOptions | الخيارات لتسليط الضوء الأيسر. |
| rightHighlightOptions | HighlightOptions | الخيارات لتسليط الضوء الأيمن. |

### انظر أيضًا

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_5}

ينشئ مثيلاً جديدًا من الفئة [`SearchOptions`](../../searchoptions) التي تُستخدم للبحث باستخدام خيارات تسليط الضوء لاستخراج التسليط الضوئي الأيسر والأيمن.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| matchCase | Boolean | القيمة التي تشير إلى ما إذا كان تمييز حالة النص غير متجاهل. |
| matchWholeWord | Boolean | القيمة التي تشير إلى ما إذا كان البحث النصي يقتصر على كلمة كاملة. |
| useRegularExpression | Boolean | القيمة التي تشير إلى ما إذا تم استخدام تعبير نمطي. |
| leftHighlightOptions | HighlightOptions | الخيارات لتسليط الضوء الأيسر. |
| rightHighlightOptions | HighlightOptions | الخيارات لتسليط الضوء الأيمن. |

### انظر أيضًا

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions) {#constructor_4}

ينشئ مثيلاً جديدًا من الفئة [`SearchOptions`](../../searchoptions) التي تُستخدم للبحث باستخدام نفس خيارات تسليط الضوء لاستخراج التسليط الضوئي الأيسر والأيمن.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions highlightOptions)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| matchCase | Boolean | القيمة التي تشير إلى ما إذا كان تمييز حالة النص غير متجاهل. |
| matchWholeWord | Boolean | القيمة التي تشير إلى ما إذا كان البحث النصي يقتصر على كلمة كاملة. |
| useRegularExpression | Boolean | القيمة التي تشير إلى ما إذا تم استخدام تعبير نمطي. |
| highlightOptions | HighlightOptions | الخيارات لكلا التسليطين الضوئيين. |

### انظر أيضًا

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool) {#constructor_1}

ينشئ مثيلاً جديدًا من الفئة [`SearchOptions`](../../searchoptions) التي تُستخدم للبحث دون استخراج التسليط الضوئي.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| matchCase | Boolean | القيمة التي تشير إلى ما إذا كان تمييز حالة النص غير متجاهل. |
| matchWholeWord | Boolean | القيمة التي تشير إلى ما إذا كان البحث النصي يقتصر على كلمة كاملة. |
| useRegularExpression | Boolean | القيمة التي تشير إلى ما إذا تم استخدام تعبير نمطي. |

### انظر أيضًا

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, bool) {#constructor_2}

ينشئ مثيلاً جديدًا من الفئة [`SearchOptions`](../../searchoptions) التي تُستخدم للبحث حسب الصفحات ودون استخراج التسليط الضوئي.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| matchCase | Boolean | القيمة التي تشير إلى ما إذا كان تمييز حالة النص غير متجاهل. |
| matchWholeWord | Boolean | القيمة التي تشير إلى ما إذا كان البحث النصي يقتصر على كلمة كاملة. |
| useRegularExpression | Boolean | القيمة التي تشير إلى ما إذا تم استخدام تعبير نمطي. |
| searchByPages | Boolean | القيمة التي تشير إلى ما إذا تم إجراء البحث حسب الصفحات. |

### انظر أيضًا

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions() {#constructor}

ينشئ مثيلاً جديدًا من الفئة [`SearchOptions`](../../searchoptions) بالقيم الافتراضية. راجع الملاحظات للتفاصيل.

```csharp
public SearchOptions()
```

### ملاحظات

الخصائص التالية لها قيم افتراضية:

**[`MatchCase`](../matchcase)**

`false`

**[`MatchWholeWord`](../matchwholeword)**

`false`

**[`UseRegularExpression`](../useregularexpression)**

`false`

**[`LeftHighlightOptions`](../lefthighlightoptions)**

`null`

**[`RightHighlightOptions`](../righthighlightoptions)**

`null`

### انظر أيضًا

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

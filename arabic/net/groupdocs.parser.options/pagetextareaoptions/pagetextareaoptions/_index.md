---
title: "PageTextAreaOptions"
second_title: "GroupDocs.Parser لـ .NET API مرجع"
description: "ينشئ مثيلًا جديدًا من الفئة PageTextAreaOptionsgroupdocs.parser.options/pagetextareaoptions مع خيار استخدام OCR."
type: docs
weight: 10
url: /ar/net/groupdocs.parser.options/pagetextareaoptions/pagetextareaoptions/
---

## PageTextAreaOptions() {#constructor}

ينشئ مثيلًا جديدًا من الفئة [`PageTextAreaOptions`](../../pagetextareaoptions) مع خيار استخدام OCR.

```csharp
public PageTextAreaOptions()
```

### انظر أيضًا

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool) {#constructor_1}

ينشئ مثيلًا جديدًا من الفئة [`PageTextAreaOptions`](../../pagetextareaoptions) مع خيار استخدام OCR.

```csharp
public PageTextAreaOptions(bool useOcr)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| useOcr | Boolean | القيمة التي تشير إلى ما إذا تم استخدام وظيفة OCR لاستخراج مناطق النص. |

### انظر أيضًا

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool, OcrOptions) {#constructor_2}

ينشئ مثيلًا جديدًا من الفئة [`PageTextAreaOptions`](../../pagetextareaoptions) مع القدرة على تعيين خيارات OCR.

```csharp
public PageTextAreaOptions(bool useOcr, OcrOptions ocrOptions)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| useOcr | Boolean | القيمة التي تشير إلى ما إذا تم استخدام وظيفة OCR لاستخراج مناطق النص. |
| ocrOptions | OcrOptions | الخيارات الإضافية لوظيفة OCR. |

### انظر أيضًا

* class [OcrOptions](../../ocroptions)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string) {#constructor_3}

ينشئ مثيلًا جديدًا من الفئة [`PageTextAreaOptions`](../../pagetextareaoptions) مع التعبير النمطي. يتم تعيين الخيارات الأخرى افتراضيًا (انظر الملاحظات للتفاصيل).

```csharp
public PageTextAreaOptions(string expression)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| expression | سلسلة | التعبير النمطي. |

### ملاحظات

الخصائص التالية لها قيم افتراضية:

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

**[`Rectangle`](../../pageareaoptions/rectangle)**

`null`

### انظر أيضًا

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle) {#constructor_6}

يقوم بإنشاء نسخة جديدة من الفئة [`PageTextAreaOptions`](../../pagetextareaoptions) مع التعبير النمطي والمساحة المستطيلة. يتم تعيين الخيارات الأخرى بشكل افتراضي (انظر الملاحظات للتفاصيل).

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| expression | سلسلة | التعبير النمطي. |
| rectangle | Rectangle | المنطقة المستطيلة التي تحتوي على مناطق الصفحة. |

### ملاحظات

الخصائص التالية لها قيم افتراضية:

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

### انظر أيضًا

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle, double) {#constructor_7}

يقوم بإنشاء نسخة جديدة من الفئة [`PageTextAreaOptions`](../../pagetextareaoptions) مع التعبير النمطي والمساحة المستطيلة وحجم الحد المتجاهل. يتم تعيين الخيارات الأخرى بشكل افتراضي (انظر الملاحظات للتفاصيل).

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle, double rectangleTolerance)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| expression | سلسلة | التعبير النمطي. |
| rectangle | Rectangle | المنطقة المستطيلة التي تحتوي على مناطق الصفحة. |
| rectangleTolerance | Double | حجم الحد الذي يتم تجاهله عند التقاطه بواسطة المنطقة المستطيلة. يتم قياسه بنسبة من ارتفاع عنصر النص. |

### انظر أيضًا

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle) {#constructor_4}

يقوم بإنشاء نسخة جديدة من الفئة [`PageTextAreaOptions`](../../pagetextareaoptions).

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| expression | سلسلة | التعبير النمطي. |
| matchCase | Boolean | القيمة التي تشير إلى ما إذا كان تمييز حالة النص غير متجاهل. |
| uniteSegments | Boolean | القيمة التي تشير إلى ما إذا كانت القطاعات موحدة. |
| ignoreFormatting | Boolean | القيمة التي تشير إلى ما إذا كان تنسيق النص متجاهلاً. |
| rectangle | Rectangle | المنطقة المستطيلة التي تحتوي على مناطق الصفحة. |

### انظر أيضًا

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle, double) {#constructor_5}

يقوم بإنشاء نسخة جديدة من الفئة [`PageTextAreaOptions`](../../pagetextareaoptions) مع حجم الحد المتجاهل.

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| expression | سلسلة | التعبير النمطي. |
| matchCase | Boolean | القيمة التي تشير إلى ما إذا كان تمييز حالة النص غير متجاهل. |
| uniteSegments | Boolean | القيمة التي تشير إلى ما إذا كانت القطاعات موحدة. |
| ignoreFormatting | Boolean | القيمة التي تشير إلى ما إذا كان تنسيق النص متجاهلاً. |
| rectangle | Rectangle | المنطقة المستطيلة التي تحتوي على مناطق الصفحة. |
| rectangleTolerance | Double | حجم الحد الذي يتم تجاهله عند التقاطه بواسطة المنطقة المستطيلة. يتم قياسه بنسبة من ارتفاع عنصر النص. |

### انظر أيضًا

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

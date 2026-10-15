---
title: "OcrOptions"
second_title: "GroupDocs.Parser لـ .NET API مرجع"
description: "ينشئ مثيلًا جديدًا من الفئة OcrOptionsgroupdocs.parser.options/ocroptions مع المنطقة المستطيلة."
type: docs
weight: 10
url: /ar/net/groupdocs.parser.options/ocroptions/ocroptions/
---

## OcrOptions() {#constructor}

ينشئ مثيلًا جديدًا من الفئة [`OcrOptions`](../../ocroptions) مع المنطقة المستطيلة.

```csharp
public OcrOptions()
```

### انظر أيضًا

* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(PagePreviewOptions) {#constructor_6}

ينشئ مثيلًا جديدًا من الفئة [`OcrOptions`](../../ocroptions) مع المنطقة المستطيلة.

```csharp
public OcrOptions(PagePreviewOptions pagePreviewOptions)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| pagePreviewOptions | PagePreviewOptions | مثال من الفئة [`PagePreviewOptions`](../pagepreviewoptions) التي تحدد الخصائص لتوليد معاينة صفحة المستند. |

### انظر أيضًا

* class [PagePreviewOptions](../../pagepreviewoptions)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle) {#constructor_1}

ينشئ مثيلًا جديدًا من الفئة [`OcrOptions`](../../ocroptions) مع المنطقة المستطيلة.

```csharp
public OcrOptions(Rectangle rectangle)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| rectangle | Rectangle | المنطقة المستطيلة التي تقيد مساحة الصفحة المستخدمة للتعرف على النص. |

### انظر أيضًا

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(OcrEventHandler) {#constructor_5}

ينشئ مثيلًا جديدًا من الفئة [`OcrOptions`](../../ocroptions) مع كائن [`OcrEventHandler`](../../ocreventhandler).

```csharp
public OcrOptions(OcrEventHandler handler)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| handler | OcrEventHandler | مثال على [`OcrEventHandler`](../../ocreventhandler) لالتقاط أحداث OCR. |

### انظر أيضًا

* class [OcrEventHandler](../../ocreventhandler)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle, OcrEventHandler) {#constructor_2}

يُنشئ مثلاً جديداً للفئة [`OcrOptions`](../../ocroptions) مع مساحة مستطيلة وكائن [`OcrEventHandler`](../../ocreventhandler).

```csharp
public OcrOptions(Rectangle rectangle, OcrEventHandler handler)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| rectangle | Rectangle | المنطقة المستطيلة التي تقيد مساحة الصفحة المستخدمة للتعرف على النص. |
| handler | OcrEventHandler | مثال على [`OcrEventHandler`](../../ocreventhandler) لالتقاط أحداث OCR. |

### انظر أيضًا

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrEventHandler](../../ocreventhandler)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle, OcrEventHandler, PagePreviewOptions, bool) {#constructor_3}

يُنشئ مثلاً جديداً للفئة [`OcrOptions`](../../ocroptions).

```csharp
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, 
    PagePreviewOptions pagePreviewOptions, bool useSpellCheker)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| rectangle | Rectangle | المنطقة المستطيلة التي تقيد مساحة الصفحة المستخدمة للتعرف على النص. |
| handler | OcrEventHandler | مثال على [`OcrEventHandler`](../../ocreventhandler) لالتقاط أحداث OCR. |
| pagePreviewOptions | PagePreviewOptions | مثال من الفئة [`PagePreviewOptions`](../pagepreviewoptions) التي تحدد الخصائص لتوليد معاينة صفحة المستند. |
| useSpellCheker | Boolean | القيمة التي تشير إلى ما إذا كان مدقق الإملاء مستخدمًا. |

### انظر أيضًا

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrEventHandler](../../ocreventhandler)
* class [PagePreviewOptions](../../pagepreviewoptions)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle, OcrEventHandler, PagePreviewOptions, bool, Language) {#constructor_4}

يُنشئ مثلاً جديداً للفئة [`OcrOptions`](../../ocroptions).

```csharp
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, 
    PagePreviewOptions pagePreviewOptions, bool useSpellCheker, Language language)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| rectangle | Rectangle | المنطقة المستطيلة التي تقيد مساحة الصفحة المستخدمة للتعرف على النص. |
| handler | OcrEventHandler | مثال على [`OcrEventHandler`](../../ocreventhandler) لالتقاط أحداث OCR. |
| pagePreviewOptions | PagePreviewOptions | مثال من الفئة [`PagePreviewOptions`](../pagepreviewoptions) التي تحدد الخصائص لتوليد معاينة صفحة المستند. |
| useSpellCheker | Boolean | القيمة التي تشير إلى ما إذا كان مدقق الإملاء مستخدمًا. |
| language | اللغة | اللغة المستخدمة في OCR. |

### انظر أيضًا

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrEventHandler](../../ocreventhandler)
* class [PagePreviewOptions](../../pagepreviewoptions)
* enum [Language](../../language)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

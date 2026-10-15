---
title: "PageTextAreaOptions"
second_title: "GroupDocs.Parser for .NET API 参考"
description: "使用 OCR 选项初始化 PageTextAreaOptionsgroupdocs.parser.options/pagetextareaoptions 类的新实例。"
type: docs
weight: 10
url: /zh/net/groupdocs.parser.options/pagetextareaoptions/pagetextareaoptions/
---

## PageTextAreaOptions() {#constructor}

使用 OCR 选项初始化 [`PageTextAreaOptions`](../../pagetextareaoptions) 类的新实例。

```csharp
public PageTextAreaOptions()
```

### 另请参见

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool) {#constructor_1}

使用 OCR 选项初始化 [`PageTextAreaOptions`](../../pagetextareaoptions) 类的新实例。

```csharp
public PageTextAreaOptions(bool useOcr)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| useOcr | Boolean | 指示是否使用 OCR 功能提取文本区域的值。 |

### 另请参见

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool, OcrOptions) {#constructor_2}

初始化 [`PageTextAreaOptions`](../../pagetextareaoptions) 类的新实例，以便设置 OCR 选项。

```csharp
public PageTextAreaOptions(bool useOcr, OcrOptions ocrOptions)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| useOcr | Boolean | 指示是否使用 OCR 功能提取文本区域的值。 |
| ocrOptions | OcrOptions | OCR 功能的附加选项。 |

### 另请参见

* class [OcrOptions](../../ocroptions)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string) {#constructor_3}

使用正则表达式初始化 [`PageTextAreaOptions`](../../pagetextareaoptions) 类的新实例。其他选项使用默认设置（详情请参阅备注）。

```csharp
public PageTextAreaOptions(string expression)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 表达式 | 字符串 | 正则表达式。 |

### 备注

以下属性具有默认值：

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

**[`Rectangle`](../../pageareaoptions/rectangle)**

`null`

### 另请参见

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle) {#constructor_6}

使用正则表达式和矩形区域初始化 [`PageTextAreaOptions`](../../pagetextareaoptions) 类的新实例。其他选项使用默认设置（详情请参阅备注）。

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 表达式 | 字符串 | 正则表达式。 |
| rectangle | 矩形 | 包含页面区域的矩形区域。 |

### 备注

以下属性具有默认值：

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

### 另请参见

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle, double) {#constructor_7}

使用正则表达式、矩形区域和忽略边框的大小初始化 [`PageTextAreaOptions`](../../pagetextareaoptions) 类的新实例。其他选项使用默认设置（详情请参阅备注）。

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle, double rectangleTolerance)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 表达式 | 字符串 | 正则表达式。 |
| rectangle | 矩形 | 包含页面区域的矩形区域。 |
| rectangleTolerance | Double | 在矩形区域捕获时被忽略的边框大小。它以文本项高度的比例来衡量。 |

### 另请参见

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle) {#constructor_4}

初始化 [`PageTextAreaOptions`](../../pagetextareaoptions) 类的新实例。

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 表达式 | 字符串 | 正则表达式。 |
| matchCase | Boolean | 指示文本大小写是否未被忽略的值。 |
| uniteSegments | Boolean | 指示段是否已合并的值。 |
| ignoreFormatting | Boolean | 指示文本格式是否被忽略的值。 |
| rectangle | 矩形 | 包含页面区域的矩形区域。 |

### 另请参见

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle, double) {#constructor_5}

使用被忽略边框的大小初始化 [`PageTextAreaOptions`](../../pagetextareaoptions) 类的新实例。

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 表达式 | 字符串 | 正则表达式。 |
| matchCase | Boolean | 指示文本大小写是否未被忽略的值。 |
| uniteSegments | Boolean | 指示段是否已合并的值。 |
| ignoreFormatting | Boolean | 指示文本格式是否被忽略的值。 |
| rectangle | 矩形 | 包含页面区域的矩形区域。 |
| rectangleTolerance | Double | 在矩形区域捕获时被忽略的边框大小。它以文本项高度的比例来衡量。 |

### 另请参见

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

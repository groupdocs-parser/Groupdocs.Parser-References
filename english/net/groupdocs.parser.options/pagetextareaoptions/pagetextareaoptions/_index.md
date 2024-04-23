---
title: PageTextAreaOptions
second_title: GroupDocs.Parser for .NET API Reference
description: Initializes a new instance of the PageTextAreaOptionsgroupdocs.parser.options/pagetextareaoptions class with the OCR usage option.
type: docs
weight: 10
url: /net/groupdocs.parser.options/pagetextareaoptions/pagetextareaoptions/
---
## PageTextAreaOptions(bool) {#constructor}

Initializes a new instance of the [`PageTextAreaOptions`](../../pagetextareaoptions) class with the OCR usage option.

```csharp
public PageTextAreaOptions(bool useOcr)
```

| Parameter | Type | Description |
| --- | --- | --- |
| useOcr | Boolean | The value that indicates whether OCR functionality is used to extract text areas. |

### See Also

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool, OcrOptions) {#constructor_1}

Initializes a new instance of the [`PageTextAreaOptions`](../../pagetextareaoptions) class with the ability to set OCR options.

```csharp
public PageTextAreaOptions(bool useOcr, OcrOptions ocrOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| useOcr | Boolean | The value that indicates whether OCR functionality is used to extract text areas. |
| ocrOptions | OcrOptions | The additional options for OCR functionality. |

### See Also

* class [OcrOptions](../../ocroptions)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string) {#constructor_2}

Initializes a new instance of the [`PageTextAreaOptions`](../../pagetextareaoptions) class with the regular expression. Other options are set by default (see remarks for details).

```csharp
public PageTextAreaOptions(string expression)
```

| Parameter | Type | Description |
| --- | --- | --- |
| expression | String | The regular expression. |

### Remarks

The following properties have default values:

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

**[`Rectangle`](../../pageareaoptions/rectangle)**

`null`

### See Also

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle) {#constructor_5}

Initializes a new instance of the [`PageTextAreaOptions`](../../pagetextareaoptions) class with the regular expression and rectangular area. Other options are set by default (see remarks for details).

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle)
```

| Parameter | Type | Description |
| --- | --- | --- |
| expression | String | The regular expression. |
| rectangle | Rectangle | The rectangular area that contains page areas. |

### Remarks

The following properties have default values:

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

### See Also

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle, double) {#constructor_6}

Initializes a new instance of the [`PageTextAreaOptions`](../../pagetextareaoptions) class with the regular expression, rectangular area and the size of the ignored border. Other options are set by default (see remarks for details).

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle, double rectangleTolerance)
```

| Parameter | Type | Description |
| --- | --- | --- |
| expression | String | The regular expression. |
| rectangle | Rectangle | The rectangular area that contains page areas. |
| rectangleTolerance | Double | The size of the border that is ignored when captured by the rectangular area. It's measured by the fraction of a text item height. |

### See Also

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle) {#constructor_3}

Initializes a new instance of the [`PageTextAreaOptions`](../../pagetextareaoptions) class.

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle)
```

| Parameter | Type | Description |
| --- | --- | --- |
| expression | String | The regular expression. |
| matchCase | Boolean | The value that indicates whether a text case isn't ignored. |
| uniteSegments | Boolean | The value that indicates whether segments are united. |
| ignoreFormatting | Boolean | The value that indicates whether text formatting is ignored. |
| rectangle | Rectangle | The rectangular area that contains page areas. |

### See Also

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle, double) {#constructor_4}

Initializes a new instance of the [`PageTextAreaOptions`](../../pagetextareaoptions) class with the size of the ignored border.

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```

| Parameter | Type | Description |
| --- | --- | --- |
| expression | String | The regular expression. |
| matchCase | Boolean | The value that indicates whether a text case isn't ignored. |
| uniteSegments | Boolean | The value that indicates whether segments are united. |
| ignoreFormatting | Boolean | The value that indicates whether text formatting is ignored. |
| rectangle | Rectangle | The rectangular area that contains page areas. |
| rectangleTolerance | Double | The size of the border that is ignored when captured by the rectangular area. It's measured by the fraction of a text item height. |

### See Also

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.parser.dll -->

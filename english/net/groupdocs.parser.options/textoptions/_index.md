---
title: TextOptions
second_title: GroupDocs.Parser for .NET API Reference
description: Provides the options which are used for text extraction.
type: docs
weight: 580
url: /net/groupdocs.parser.options/textoptions/
---
## TextOptions class

Provides the options which are used for text extraction.

```csharp
public sealed class TextOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [TextOptions](textoptions)(bool) | Initializes a new instance of the [`TextOptions`](../textoptions) class. |

## Properties

| Name | Description |
| --- | --- |
| [UseRawModeIfPossible](../../groupdocs.parser.options/textoptions/userawmodeifpossible) { get; } | Gets the value that indicates whether the raw mode is used. |

### Remarks

An instance of [`TextOptions`](../textoptions) class is used as parameter in [`GetText`](../../groupdocs.parser/parser/gettext) and [`GetText`](../../groupdocs.parser/parser/gettext) methods. See the usage examples there.

It's used to specify the raw mode of text extraction. A text in this mode is extracted in a non-accurate way but faster than in the standard mode. If the raw mode doesn't support the document format, then this parameter is ignored and the standard mode is used.

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### See Also

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.parser.dll -->
---
title: HighlightOptions
second_title: GroupDocs.Parser for .NET API Reference
description: Provides the options which are used to extract a highlight a block of text aroud found text in search scenarios.
type: docs
weight: 400
url: /net/groupdocs.parser.options/highlightoptions/
---
## HighlightOptions class

Provides the options which are used to extract a highlight (a block of text aroud found text in search scenarios).

```csharp
public sealed class HighlightOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [HighlightOptions](highlightoptions#constructor)(int) | Initializes a new instance of the [`HighlightOptions`](../highlightoptions) class which is used to extract a fixed-length highlight. |
| [HighlightOptions](highlightoptions#constructor_1)(int?, bool) | Initializes a new instance of the [`HighlightOptions`](../highlightoptions) class which is used to extract a line-limited highlight. |
| [HighlightOptions](highlightoptions#constructor_2)(int?, int) | Initializes a new instance of the [`HighlightOptions`](../highlightoptions) class which is used to extract a highlight with the fixed word count. |
| [HighlightOptions](highlightoptions#constructor_3)(int?, int?, bool) | Initializes a new instance of the [`HighlightOptions`](../highlightoptions) class. |

## Properties

| Name | Description |
| --- | --- |
| [IsLineLimited](../../groupdocs.parser.options/highlightoptions/islinelimited) { get; } | Gets value that indicates whether highlight extraction is limited by the start (or the end) of a text line. |
| [MaxLength](../../groupdocs.parser.options/highlightoptions/maxlength) { get; } | Gets a maximum text length. |
| [WordCount](../../groupdocs.parser.options/highlightoptions/wordcount) { get; } | Gets a maximum word count. |

### Remarks

An instance of [`HighlightOptions`](../highlightoptions) class is used as parameter in [`GetHighlight`](../../groupdocs.parser/parser/gethighlight) method. See the usage examples there.

**Learn more:**

* [Extract highlights](https://docs.groupdocs.com/display/parsernet/Extract+highlights)

### See Also

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.parser.dll -->
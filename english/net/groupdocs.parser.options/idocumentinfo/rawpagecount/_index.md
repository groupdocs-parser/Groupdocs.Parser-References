---
title: RawPageCount
second_title: GroupDocs.Parser for .NET API Reference
description: Gets the total number of document raw pages.
type: docs
weight: 40
url: /net/groupdocs.parser.options/idocumentinfo/rawpagecount/
---
## IDocumentInfo.RawPageCount property

Gets the total number of document raw pages.

```csharp
public int RawPageCount { get; }
```

### Property Value

An integer value that represents a total number of raw pages.

### Remarks

Use `RawPageCount` property instead of [`PageCount`](../pagecount) property for raw text extraction. Some documents have different page numbers in accurate and raw text extraction modes. [`PageCount`](../pagecount) property may perform extra calculations which impacts on text extraction speed in raw mode.

### See Also

* interface [IDocumentInfo](../../idocumentinfo)
* namespace [GroupDocs.Parser.Options](../../idocumentinfo)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.parser.dll -->
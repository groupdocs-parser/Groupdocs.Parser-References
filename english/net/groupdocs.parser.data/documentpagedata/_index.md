---
title: DocumentPageData
second_title: GroupDocs.Parser for .NET API Reference
description: Represents data of the document page. It consists of FieldData./fielddata objects which contain field data from the document page.
type: docs
weight: 30
url: /net/groupdocs.parser.data/documentpagedata/
---
## DocumentPageData class

Represents data of the document page. It consists of [`FieldData`](../fielddata) objects which contain field data from the document page.

```csharp
public sealed class DocumentPageData : DocumentData
```

## Constructors

| Name | Description |
| --- | --- |
| [DocumentPageData](documentpagedata)(IEnumerable&lt;FieldData&gt;, int) | Initializes a new instance of the [`DocumentPageData`](../documentpagedata) class. |

## Properties

| Name | Description |
| --- | --- |
| [Count](../../groupdocs.parser.data/documentdata/count) { get; } | Gets the total number of the fields data. |
| [Item](../../groupdocs.parser.data/documentdata/item) { get; } | Gets the field data by an index. |
| [PageIndex](../../groupdocs.parser.data/documentpagedata/pageindex) { get; } | Gets the page index. |

## Methods

| Name | Description |
| --- | --- |
| [GetEnumerator](../../groupdocs.parser.data/documentdata/getenumerator)() | Returns an enumerator for the fields data. |
| [GetFieldsByName](../../groupdocs.parser.data/documentdata/getfieldsbyname)(string) | Returns the collection of field data where the name is equal to *fieldName*. |

### See Also

* class [DocumentData](../documentdata)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.parser.dll -->
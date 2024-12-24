---
title: WorksheetInfo
second_title: GroupDocs.Parser for .NET API Reference
description: Initializes a new instance of the WorksheetInfogroupdocs.parser.data/worksheetinfo class.
type: docs
weight: 10
url: /net/groupdocs.parser.data/worksheetinfo/worksheetinfo/
---
## WorksheetInfo constructor

Initializes a new instance of the [`WorksheetInfo`](../../worksheetinfo) class.

```csharp
public WorksheetInfo(int index, string name, WorksheetRange range)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The zero-based index of the worksheet. |
| name | String | A string value that represents the worksheet name. |
| range | WorksheetRange | An instance of [`WorksheetRange`](../../worksheetrange) class that represents the size of the worksheet. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | An index of the worksheet can't be negative. |
| ArgumentNullException | The size of the worksheet can't be `null`. |

### See Also

* class [WorksheetRange](../../worksheetrange)
* class [WorksheetInfo](../../worksheetinfo)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.parser.dll -->
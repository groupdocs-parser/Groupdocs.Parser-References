---
title: WorksheetInfo constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.data/worksheetinfo/__init__/
is_root: false
weight: 10
---

## __init__ {#int-System.String-groupdocs.parser.data.WorksheetRange}

Initializes a new instance of the [`WorksheetInfo`](/parser/python-net/groupdocs.parser.data/worksheetinfo) class.



```python
def __init__(self, index, name, range):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| index | int | The zero-based index of the worksheet. |
| name | System.String | A string value that represents the worksheet name. |
| range | groupdocs.parser.data.WorksheetRange | An instance of [`WorksheetRange`](/parser/python-net/groupdocs.parser.data/worksheetrange) class that represents the size of the worksheet. |
### Exceptions
| Exception | Description |
| :- | :- |
| ArgumentOutOfRangeException | An index of the worksheet can't be negative. |
| ArgumentNullException | The size of the worksheet can't be `null`. |





### See Also
* module [`groupdocs.parser.data`](../../)
* class [`WorksheetInfo`](/parser/python-net/groupdocs.parser.data/worksheetinfo)
* class [`WorksheetRange`](/parser/python-net/groupdocs.parser.data/worksheetrange)

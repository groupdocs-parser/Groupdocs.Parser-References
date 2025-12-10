---
title: get_worksheet_info method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser/parser/get_worksheet_info/
is_root: false
weight: 190
---

## get_worksheet_info {#}

Extracts the info about all worksheets in the spreadsheet.


### Returns 


A collection of instances of [`WorksheetInfo`](/parser/python-net/groupdocs.parser.data/worksheetinfo) class that contains the info about all worksheets in the spreadsheet.


```python
def get_worksheet_info(self):
    ...
```




## get_worksheet_info {#int}

Extracts the info about the worksheet.


### Returns 


An instance of [`WorksheetInfo`](/parser/python-net/groupdocs.parser.data/worksheetinfo) class that contains the info about all worksheets in the spreadsheet.


```python
def get_worksheet_info(self, worksheet_index):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| worksheet_index | int | The zero-based index of the worksheet. |



### See Also
* module [`groupdocs.parser`](../../)
* class [`Parser`](/parser/python-net/groupdocs.parser/parser)
* class [`WorksheetInfo`](/parser/python-net/groupdocs.parser.data/worksheetinfo)

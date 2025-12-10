---
title: get_worksheet_cells method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser/parser/get_worksheet_cells/
is_root: false
weight: 180
---

## get_worksheet_cells {#int}

Extracts worksheet cells.


### Returns 


A collection of instances of [`WorksheetCell`](/parser/python-net/groupdocs.parser.data/worksheetcell) class that contains the cell data.


```python
def get_worksheet_cells(self, worksheet_index):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| worksheet_index | int | The zero-based index of the worksheet. |


## get_worksheet_cells {#int-groupdocs.parser.options.WorksheetOptions}

Extracts worksheet cells using customization options.


### Returns 


A collection of instances of [`WorksheetCell`](/parser/python-net/groupdocs.parser.data/worksheetcell) class that contains the cell data.


```python
def get_worksheet_cells(self, worksheet_index, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| worksheet_index | int | The zero-based index of the worksheet. |
| options | groupdocs.parser.options.WorksheetOptions | The customization options. |



### See Also
* module [`groupdocs.parser`](../../)
* class [`Parser`](/parser/python-net/groupdocs.parser/parser)
* class [`WorksheetCell`](/parser/python-net/groupdocs.parser.data/worksheetcell)

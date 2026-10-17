---
title: get_worksheet_cells method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Extracts worksheet cells."
type: docs
url: /python-net/groupdocs.parser/parser/get_worksheet_cells/
is_root: false
weight: 1440
---


## get_worksheet_cells {#worksheet_index}

Extracts worksheet cells.

```python
def get_worksheet_cells(self, worksheet_index):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| worksheet_index | `int` | The zero-based index of the worksheet. |

**Returns:** Iterable[WorksheetCell]: A collection of instances of `WorksheetCell` class that contains the cell data.

## get_worksheet_cells {#worksheet_index-options}

Extracts worksheet cells using customization options.

```python
def get_worksheet_cells(self, worksheet_index, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| worksheet_index | `int` | The zero-based index of the worksheet. |
| options | `WorksheetOptions` | The customization options. |

**Returns:** Iterable[WorksheetCell]: A collection of instances of `WorksheetCell` containing the cell data.

### See Also
* class [`Parser`](/parser/python-net/groupdocs.parser/parser/)

---
title: get_worksheet_info method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Extracts the info about all worksheets in the spreadsheet."
type: docs
url: /python-net/groupdocs.parser/parser/get_worksheet_info/
is_root: false
weight: 1210
---


## get_worksheet_info

Extracts the info about all worksheets in the spreadsheet.

```python
def get_worksheet_info(self):
    ...
```

**Returns:** list[`WorksheetInfo`]: Collection of `WorksheetInfo` instances containing info about all worksheets in the spreadsheet.

## get_worksheet_info {#worksheet_index}

Extracts the info about the worksheet.

```python
def get_worksheet_info(self, worksheet_index):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| worksheet_index | `int` | The zero-based index of the worksheet. |

**Returns:** WorksheetInfo: An instance that contains the info about all worksheets in the spreadsheet.

### Aliases

These names call `get_worksheet_info` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_worksheet_info_int32` | `get_worksheet_info_int32(worksheet_index)` |

### See Also
* class [`Parser`](/parser/python-net/groupdocs.parser/parser/)

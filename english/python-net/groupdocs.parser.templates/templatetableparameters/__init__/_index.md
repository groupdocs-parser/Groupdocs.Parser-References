---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new instance of the TemplateTableParameters class."
type: docs
url: /python-net/groupdocs.parser.templates/templatetableparameters/__init__/
is_root: false
weight: 10
---


## __init__ {#rectangle-vertical_separators}

Initializes a new instance of the TemplateTableParameters class.

```python
def __init__(self, rectangle, vertical_separators):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| rectangle | `Rectangle` | The rectangular area that contains the table. |
| vertical_separators | `Iterable[float]` | The table column separators. |

### Example

```python
from groupdocs.parser.data import Rectangle, Point, Size
from groupdocs.parser.templates import TemplateTableParameters

table_area = Rectangle(Point(175.0, 350.0), Size(400.0, 200.0))
columns = [185.0, 370.0, 425.0, 485.0, 545.0]

params = TemplateTableParameters(table_area, columns)
```

## __init__ {#rectangle-vertical_separators-has_merged_cells-min_row_count-min_column_count-min_vertical_space}

Initializes a new instance of the TemplateTableParameters class.

```python
def __init__(self, rectangle, vertical_separators, has_merged_cells, min_row_count, min_column_count, min_vertical_space):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| rectangle | `Rectangle` | The rectangular area that contains the table. |
| vertical_separators | `Iterable[float]` | The table columns separators. |
| has_merged_cells | `Optional[bool]` | Indicates whether the table has merged cells. |
| min_row_count | `Optional[int]` | The minimum number of the table rows. |
| min_column_count | `Optional[int]` | The minimum number of the table columns. |
| min_vertical_space | `Optional[int]` | The minimum space between the table columns. |

### Example

```python
from groupdocs.parser.data import Rectangle, Point, Size
from groupdocs.parser.templates import TemplateTableParameters

table_area = Rectangle(Point(175.0, 350.0), Size(400.0, 200.0))
columns = [185.0, 370.0, 425.0, 485.0, 545.0]

params = TemplateTableParameters(table_area, columns)
```

### See Also
* class [`TemplateTableParameters`](/parser/python-net/groupdocs.parser.templates/templatetableparameters/)

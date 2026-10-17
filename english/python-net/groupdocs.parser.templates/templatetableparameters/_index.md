---
title: TemplateTableParameters class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Provides parameters for the table detection algorithms."
type: docs
url: /python-net/groupdocs.parser.templates/templatetableparameters/
is_root: false
weight: 140
---


## TemplateTableParameters class

Provides parameters for the table detection algorithms.

There are two algorithms to detect a table:

- Detect a table in the rectangular area with set columns. This algorithm is useful for simple tables (without merged columns) and provides more accurate detection.
- Detect a table in any place on the page. This is a more complex algorithm. It can detect tables in any place on the page. Additional parameters help to detect a table more correctly.

In some cases when algorithms can't detect a table or do it in a non‑accurate way, [`TemplateTableLayout`](/parser/python-net/groupdocs.parser.templates/templatetablelayout/) class is used.

The TemplateTableParameters type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.templates/templatetableparameters/__init__/#rectangle-vertical_separators) | Initializes a new instance of the TemplateTableParameters class. |
| [__init__](/parser/python-net/groupdocs.parser.templates/templatetableparameters/__init__/#rectangle-vertical_separators-has_merged_cells-min_row_count-min_column_count-min_vertical_space) | Initializes a new instance of the TemplateTableParameters class. |

### Properties
| Property | Description |
| :- | :- |
| [has_merged_cells](/parser/python-net/groupdocs.parser.templates/templatetableparameters/has_merged_cells/) | The value indicates whether the table has merged cells. True if the table has merged cells; otherwise False. None if it isn't set. |
| [min_column_count](/parser/python-net/groupdocs.parser.templates/templatetableparameters/min_column_count/) | The minimum number of the table columns; None if it isn't set. |
| [min_row_count](/parser/python-net/groupdocs.parser.templates/templatetableparameters/min_row_count/) | The minimum number of table rows. |
| [min_vertical_space](/parser/python-net/groupdocs.parser.templates/templatetableparameters/min_vertical_space/) | The minimum space between the table columns. |
| [rectangle](/parser/python-net/groupdocs.parser.templates/templatetableparameters/rectangle/) | The rectangular area that contains the table. |
| [vertical_separators](/parser/python-net/groupdocs.parser.templates/templatetableparameters/vertical_separators/) | The table columns separators. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.data import Rectangle, Point, Size
from groupdocs.parser.templates import Template, TemplateTable, TemplateTableParameters

table_area = Rectangle(Point(175.0, 350.0), Size(400.0, 200.0))
columns = [185.0, 370.0, 425.0, 485.0, 545.0]

table = TemplateTable(
    parameters=TemplateTableParameters(table_area, columns),
    name="Details",
)

template = Template([table])

with Parser("./invoice.pdf") as parser:
    data = parser.parse_by_template(template)
    if data is not None:
        fields = data.get_fields_by_name("Details")
        if fields:
            details = fields[0].page_area
            print(f"Rows extracted: {details.row_count}")
```

### See Also
* module [`groupdocs.parser.templates`](/parser/python-net/groupdocs.parser.templates/)

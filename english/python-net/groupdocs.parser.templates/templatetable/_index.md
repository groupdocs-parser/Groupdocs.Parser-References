---
title: TemplateTable class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Provides the template table."
type: docs
url: /python-net/groupdocs.parser.templates/templatetable/
is_root: false
weight: 120
---


## TemplateTable class

Provides the template table.

There are two ways to define a table:

- Using [`TemplateTableLayout`](/parser/python-net/groupdocs.parser.templates/templatetablelayout/) class. In this case the table is defined by its position on the page: rectangular area, columns and rows separators.
- Using [`TemplateTableParameters`](/parser/python-net/groupdocs.parser.templates/templatetableparameters/) class. In this case the table is detected automatically by algorithms with set parameters. See [`TemplateTableParameters`](/parser/python-net/groupdocs.parser.templates/templatetableparameters/) class for more information.

The TemplateTable type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.templates/templatetable/__init__/#layout-name) | Initializes a new TemplateTable with the specified layout and name. |
| [__init__](/parser/python-net/groupdocs.parser.templates/templatetable/__init__/#layout-name-page_width) | Initializes a TemplateTable with the given layout, name (in upper case), and page width. |
| [__init__](/parser/python-net/groupdocs.parser.templates/templatetable/__init__/#layout-name-page_width-use_upper_case_name) | Initializes a new TemplateTable. |
| [__init__](/parser/python-net/groupdocs.parser.templates/templatetable/__init__/#parameters-name) | Initializes a new TemplateTable. |
| [__init__](/parser/python-net/groupdocs.parser.templates/templatetable/__init__/#parameters-name-page_width) | Initializes a new TemplateTable. |
| [__init__](/parser/python-net/groupdocs.parser.templates/templatetable/__init__/#parameters-name-page_width-use_upper_case_name) | Initializes a new TemplateTable instance. |

### Methods
| Method | Description |
| :- | :- |
| [scale](/parser/python-net/groupdocs.parser.templates/templatetable/scale/#factor) | Scales the template item by a given factor. |
| [scale_double](/parser/python-net/groupdocs.parser.templates/templatetable/scale_double/) |  |

### Properties
| Property | Description |
| :- | :- |
| [layout](/parser/python-net/groupdocs.parser.templates/templatetable/layout/) | The table layout. |
| [parameters](/parser/python-net/groupdocs.parser.templates/templatetable/parameters/) | The parameters used to detect the table in automatic mode. Returns an instance of [`TemplateTableParameters`](/parser/python-net/groupdocs.parser.templates/templatetableparameters/) or `None` if not set. |
| [name](/parser/python-net/groupdocs.parser.templates/templateitem/name/) | The name of the template item. Uppercase string value representing the template item's name. (inherited from [`TemplateItem`](/parser/python-net/groupdocs.parser.templates/templateitem/)) |
| [page_width](/parser/python-net/groupdocs.parser.templates/templateitem/page_width/) | The width of the page in pixels; None if the page width is unknown. (inherited from [`TemplateItem`](/parser/python-net/groupdocs.parser.templates/templateitem/)) |
| [use_upper_case_name](/parser/python-net/groupdocs.parser.templates/templateitem/use_upper_case_name/) | The property returns a boolean value that indicates whether a Name was converted to UPPER CASE. (inherited from [`TemplateItem`](/parser/python-net/groupdocs.parser.templates/templateitem/)) |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.data import Rectangle, Point, Size
from groupdocs.parser.templates import (
    Template,
    TemplateTable,
    TemplateTableParameters,
)

table_area = Rectangle(Point(175.0, 350.0), Size(400.0, 200.0))
columns = [185.0, 370.0, 425.0, 485.0, 545.0]

table = TemplateTable(
    parameters=TemplateTableParameters(table_area, columns),
    name="Details",
)

template = Template([table])

with Parser("./invoice.pdf") as parser:
    data = parser.parse_by_template(template)
    if data:
        fields = data.get_fields_by_name("Details")
        if fields:
            details = fields[0].page_area
            print(f"Rows extracted: {details.row_count}")
```

### See Also
* module [`groupdocs.parser.templates`](/parser/python-net/groupdocs.parser.templates/)

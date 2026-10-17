---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new TemplateTable with the specified layout and name."
type: docs
url: /python-net/groupdocs.parser.templates/templatetable/__init__/
is_root: false
weight: 10
---


## __init__ {#layout-name}

Initializes a new TemplateTable with the specified layout and name.

```python
def __init__(self, layout, name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| layout | `TemplateTableLayout` | The table layout. |
| name | `str` | The table name. |

## __init__ {#layout-name-page_width}

Initializes a TemplateTable with the given layout, name (in upper case), and page width.

```python
def __init__(self, layout, name, page_width):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| layout | `TemplateTableLayout` | The table layout. |
| name | `str` | The table name. |
| page_width | `Optional[float]` | The width of the page that was used to create the template item. |

### Example

```python
from groupdocs.parser.templates import TemplateTable, TemplateTableLayout, Template

layout = TemplateTableLayout([50.0, 95.0, 275.0], [325.0, 340.0, 365.0])
table = TemplateTable(layout, "DETAILS", None)

template = Template([table])
```

## __init__ {#layout-name-page_width-use_upper_case_name}

Initializes a new TemplateTable.

```python
def __init__(self, layout, name, page_width, use_upper_case_name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| layout | `TemplateTableLayout` | The table layout. |
| name | `str` | The table name. |
| page_width | `Optional[float]` | The width of the page that was used to create the template item. |
| use_upper_case_name | `bool` | Indicates whether a `name` is converted to UPPER CASE. |

## __init__ {#parameters-name}

Initializes a new TemplateTable.

```python
def __init__(self, parameters, name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| parameters | `TemplateTableParameters` | The parameters to detect the table in the automatic mode. |
| name | `str` | The table name. |

### Example

```python
    from groupdocs.parser import Parser
    from groupdocs.parser.data import Rectangle, Point, Size
    from groupdocs.parser.templates import (
        Template,
        TemplateItem,
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
        if data is not None:
            fields = data.get_fields_by_name("Details")
            if fields:
                details = fields[0].page_area
                print(f"Rows extracted: {details.row_count}")
    ```

## __init__ {#parameters-name-page_width}

Initializes a new TemplateTable.

```python
def __init__(self, parameters, name, page_width):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| parameters | `TemplateTableParameters` | The parameters to detect the table in the automatic mode. |
| name | `str` | The table name. |
| page_width | `Optional[float]` | The width of the page that was used to create the template item. |

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
        if data is not None:
            fields = data.get_fields_by_name("Details")
            if fields:
                details = fields[0].page_area
                print(f"Rows extracted: {details.row_count}")
    ```

## __init__ {#parameters-name-page_width-use_upper_case_name}

Initializes a new TemplateTable instance.

```python
def __init__(self, parameters, name, page_width, use_upper_case_name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| parameters | `TemplateTableParameters` | The parameters to detect the table in the automatic mode. |
| name | `str` | The table name. |
| page_width | `Optional[float]` | The width of the page that was used to create the template item. |
| use_upper_case_name | `bool` | Indicates whether the `name` is converted to upper case. |

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
    if data is not None:
        fields = data.get_fields_by_name("Details")
        if fields:
            details = fields[0].page_area
            print(f"Rows extracted: {details.row_count}")
```

### See Also
* class [`TemplateTable`](/parser/python-net/groupdocs.parser.templates/templatetable/)

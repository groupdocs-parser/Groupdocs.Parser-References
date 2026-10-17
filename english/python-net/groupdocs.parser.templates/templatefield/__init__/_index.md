---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new TemplateField instance."
type: docs
url: /python-net/groupdocs.parser.templates/templatefield/__init__/
is_root: false
weight: 10
---


## __init__ {#position-name}

Initializes a new TemplateField instance.

```python
def __init__(self, position, name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| position | `TemplatePosition` | The field position. |
| name | `str` | The field name. |

### Example

```python
from groupdocs.parser.templates import TemplateField, TemplateRegexPosition

field = TemplateField(
    TemplateRegexPosition(r"Invoice Number\s+(?<value>[A-Z0-9\-]+)"),
    "InvoiceNumber",
)
```

## __init__ {#position-name-page_width}

Initializes a new TemplateField.

```python
def __init__(self, position, name, page_width):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| position | `TemplatePosition` | The field position. |
| name | `str` | The field name. |
| page_width | `Optional[float]` | The width of the page that was used to create the template item. |

### Example

```python
from groupdocs.parser.templates import TemplateField, TemplateFixedPosition
from groupdocs.parser.data import Rectangle, Point, Size

field = TemplateField(
    TemplateFixedPosition(Rectangle(Point(35.0, 135.0), Size(100.0, 10.0))),
    "CompanyName",
)
```

## __init__ {#position-name-page_width-use_upper_case_name}

Initializes a new TemplateField.

```python
def __init__(self, position, name, page_width, use_upper_case_name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| position | `TemplatePosition` | The field position. |
| name | `str` | The field name. |
| page_width | `Optional[float]` | The width of the page that was used to create the template item. |
| use_upper_case_name | `bool` | Indicates whether the `name` is converted to upper case. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.templates import Template, TemplateField, TemplateRegexPosition

template = Template([
    TemplateField(
        TemplateRegexPosition(r"Invoice Number\s+(?<value>[A-Z0-9\-]+)"),
        "InvoiceNumber",
    )
])

with Parser("./invoice.pdf") as parser:
    data = parser.parse_by_template(template)
    if data is not None:
        fields = data.get_fields_by_name("InvoiceNumber")
        if fields:
            print(f"Invoice number: {fields[0].text}")
```

### See Also
* class [`TemplateField`](/parser/python-net/groupdocs.parser.templates/templatefield/)

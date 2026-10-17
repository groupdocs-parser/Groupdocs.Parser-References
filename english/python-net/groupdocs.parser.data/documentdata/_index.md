---
title: DocumentData class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Represents data of the document."
type: docs
url: /python-net/groupdocs.parser.data/documentdata/
is_root: false
weight: 30
---


## DocumentData class

Represents data of the document.

An instance of [`DocumentData`](/parser/python-net/groupdocs.parser.data/documentdata/) is returned by [`Parser.parse_by_template`](/parser/python-net/groupdocs.parser/parser/parse_by_template/) and [`Parser.parse_form`](/parser/python-net/groupdocs.parser/parser/parse_form/). See the usage examples there.

The DocumentData type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.data/documentdata/__init__/#fields) | Initializes a new instance of the [`DocumentData`](/parser/python-net/groupdocs.parser.data/documentdata/) class. |
| [__init__](/parser/python-net/groupdocs.parser.data/documentdata/__init__/#template-fields) | Initializes a new instance of the [`DocumentData`](/parser/python-net/groupdocs.parser.data/documentdata/) class. |

### Methods
| Method | Description |
| :- | :- |
| [get](/parser/python-net/groupdocs.parser.data/documentdata/get/) |  |
| [get_enumerator](/parser/python-net/groupdocs.parser.data/documentdata/get_enumerator/) | Returns an iterator for the fields data. |
| [get_fields_by_name](/parser/python-net/groupdocs.parser.data/documentdata/get_fields_by_name/#field_name) | Returns the collection of field data where the name is equal to `field_name`. |
| [get_fields_by_name_file](/parser/python-net/groupdocs.parser.data/documentdata/get_fields_by_name_file/) |  |
| [get_fields_by_name_string](/parser/python-net/groupdocs.parser.data/documentdata/get_fields_by_name_string/) |  |
| [get_int32](/parser/python-net/groupdocs.parser.data/documentdata/get_int32/) |  |

### Properties
| Property | Description |
| :- | :- |
| [count](/parser/python-net/groupdocs.parser.data/documentdata/count/) | The total number of fields data. |
| [template](/parser/python-net/groupdocs.parser.data/documentdata/template/) | The template. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.templates import Template, TemplateField, TemplateFixedPosition
from groupdocs.parser.data import Rectangle, Point, Size

template = Template([
    TemplateField(
        TemplateFixedPosition(Rectangle(Point(35.0, 135.0), Size(100.0, 10.0))),
        "CompanyName",
    ),
    TemplateField(
        TemplateFixedPosition(Rectangle(Point(440.0, 115.0), Size(110.0, 15.0))),
        "InvoiceNumber",
    ),
])

with Parser("./invoice.pdf") as parser:
    data = parser.parse_by_template(template)
    if data is None:
        print("Parsing by template isn't supported for this format.")
    else:
        for i in range(data.count):
            field = data[i]
            print(f"{field.name}: {field.text}")
```

### See Also
* module [`groupdocs.parser.data`](/parser/python-net/groupdocs.parser.data/)

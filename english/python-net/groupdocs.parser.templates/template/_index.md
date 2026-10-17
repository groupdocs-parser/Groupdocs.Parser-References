---
title: Template class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Provides the document page template consisting of TemplateItem objects that represent items such as text fields and table definitions."
type: docs
url: /python-net/groupdocs.parser.templates/template/
is_root: false
weight: 10
---


## Template class

Provides the document page template consisting of [`TemplateItem`](/parser/python-net/groupdocs.parser.templates/templateitem/) objects that represent items such as text fields and table definitions.

Learn more:
- https://docs.groupdocs.com/display/parsernet/Working+with+templates

The Template type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.templates/template/__init__/#items) | Initializes a new Template. |
| [__init__](/parser/python-net/groupdocs.parser.templates/template/__init__/#items-options) | Initializes a new instance of the Template class with template options. |

### Methods
| Method | Description |
| :- | :- |
| [get](/parser/python-net/groupdocs.parser.templates/template/get/) |  |
| [get_enumerator](/parser/python-net/groupdocs.parser.templates/template/get_enumerator/) | Returns an enumerator for template items. |
| [get_int32](/parser/python-net/groupdocs.parser.templates/template/get_int32/) |  |
| [load](/parser/python-net/groupdocs.parser.templates/template/load/#file_path) | Loads a template from a file. |
| [load](/parser/python-net/groupdocs.parser.templates/template/load/#stream) | Loads a template from a stream. |
| [load_file](/parser/python-net/groupdocs.parser.templates/template/load_file/) |  |
| [load_stream](/parser/python-net/groupdocs.parser.templates/template/load_stream/) |  |
| [load_streams](/parser/python-net/groupdocs.parser.templates/template/load_streams/) |  |
| [load_string](/parser/python-net/groupdocs.parser.templates/template/load_string/) |  |
| [save](/parser/python-net/groupdocs.parser.templates/template/save/#file_path) | Saves a template to a file. |
| [save](/parser/python-net/groupdocs.parser.templates/template/save/#stream) | Saves a template to a stream. |
| [save_file](/parser/python-net/groupdocs.parser.templates/template/save_file/) |  |
| [save_stream](/parser/python-net/groupdocs.parser.templates/template/save_stream/) |  |
| [save_streams](/parser/python-net/groupdocs.parser.templates/template/save_streams/) |  |
| [save_string](/parser/python-net/groupdocs.parser.templates/template/save_string/) |  |

### Properties
| Property | Description |
| :- | :- |
| [count](/parser/python-net/groupdocs.parser.templates/template/count/) | The total number of template items. |
| [is_ocr_compatible](/parser/python-net/groupdocs.parser.templates/template/is_ocr_compatible/) | The value indicating whether the template is compatible with OCR. |
| [options](/parser/python-net/groupdocs.parser.templates/template/options/) | The template options. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.templates import Template, TemplateField, TemplateRegexPosition

template = Template([
    TemplateField(
        TemplateRegexPosition(r"Invoice Number\s+(?<value>[A-Z0-9\\-]+)"),
        "InvoiceNumber",
    )
])

with Parser("./invoice.pdf") as parser:
    data = parser.parse_by_template(template)
    if data:
        print(data.get_fields_by_name("InvoiceNumber")[0].text)
```

### See Also
* module [`groupdocs.parser.templates`](/parser/python-net/groupdocs.parser.templates/)

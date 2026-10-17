---
title: TemplateRegexPosition class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Provides a template field position which uses a regular expression."
type: docs
url: /python-net/groupdocs.parser.templates/templateregexposition/
is_root: false
weight: 110
---


## TemplateRegexPosition class

Provides a template field position which uses a regular expression.

The position extracts the entire match by default. To extract a specific capture group, include a named group `value` in the pattern; only the content of that group will be returned as the field value.

The TemplateRegexPosition type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.templates/templateregexposition/__init__/#expression) | Initializes a new TemplateRegexPosition with the specified regular expression. |
| [__init__](/parser/python-net/groupdocs.parser.templates/templateregexposition/__init__/#expression-match_case) | Initializes a new TemplateRegexPosition instance. |

### Properties
| Property | Description |
| :- | :- |
| [expression](/parser/python-net/groupdocs.parser.templates/templateregexposition/expression/) | The regular expression used to locate values. |
| [match_case](/parser/python-net/groupdocs.parser.templates/templateregexposition/match_case/) | The value indicates whether text case is not ignored. |

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
    if data:
        fields = data.get_fields_by_name("InvoiceNumber")
        if fields:
            print(f"Invoice number: {fields[0].text}")
```

### See Also
* module [`groupdocs.parser.templates`](/parser/python-net/groupdocs.parser.templates/)

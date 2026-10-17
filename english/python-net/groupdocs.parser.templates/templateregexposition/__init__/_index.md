---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new TemplateRegexPosition with the specified regular expression."
type: docs
url: /python-net/groupdocs.parser.templates/templateregexposition/__init__/
is_root: false
weight: 10
---


## __init__ {#expression}

Initializes a new TemplateRegexPosition with the specified regular expression.

```python
def __init__(self, expression):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| expression | `str` | The regular expression. |

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
            invoice_number = fields[0].text
            print(f"Invoice number: {invoice_number}")
```

## __init__ {#expression-match_case}

Initializes a new TemplateRegexPosition instance.

```python
def __init__(self, expression, match_case):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| expression | `str` | The regular expression. |
| match_case | `bool` | Indicates whether text case is considered (True) or ignored (False). |

### Example

```python
from groupdocs.parser.templates import Template, TemplateField, TemplateRegexPosition

position = TemplateRegexPosition(r"Invoice Number\s+(?<value>[A-Z0-9\-]+)")
field = TemplateField(position, "InvoiceNumber")
template = Template([field])
```

### See Also
* class [`TemplateRegexPosition`](/parser/python-net/groupdocs.parser.templates/templateregexposition/)

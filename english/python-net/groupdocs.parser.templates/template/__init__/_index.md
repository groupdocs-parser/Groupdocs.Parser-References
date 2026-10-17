---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new Template."
type: docs
url: /python-net/groupdocs.parser.templates/template/__init__/
is_root: false
weight: 10
---


## __init__ {#items}

Initializes a new Template.

```python
def __init__(self, items):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| items | `Iterable[TemplateItem]` | The collection of TemplateItem objects. |

### Example

```python
from groupdocs.parser.templates import Template, TemplateField, TemplateRegexPosition

template = Template([
    TemplateField(TemplateRegexPosition(r"From"), "From"),
    TemplateField(TemplateRegexPosition(r"FromCompany"), "FromCompany"),
    TemplateField(TemplateRegexPosition(r"FromAddress"), "FromAddress"),
])
```

## __init__ {#items-options}

Initializes a new instance of the Template class with template options.

```python
def __init__(self, items, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| items | `Iterable[TemplateItem]` | The collection of TemplateItem objects. |
| options | `TemplateOptions` | The template options. |

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
* class [`Template`](/parser/python-net/groupdocs.parser.templates/template/)

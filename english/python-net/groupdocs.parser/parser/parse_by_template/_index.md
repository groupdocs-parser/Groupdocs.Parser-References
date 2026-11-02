---
title: parse_by_template method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Parses the document by the user-generated template."
type: docs
url: /python-net/groupdocs.parser/parser/parse_by_template/
is_root: false
weight: 1220
---


## parse_by_template {#template}

Parses the document by the user-generated template.

Learn more:
- [Parse data from documents](https://docs.groupdocs.com/parser/python-net/parse-data-from-documents/)
- [Working with templates](https://docs.groupdocs.com/parser/python-net/working-with-templates/)

```python
def parse_by_template(self, template):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| template | `Template` | The user-generated template. |

**Returns:** DocumentData or None: An instance of `DocumentData` that contains the extracted data, or `None` if parsing by template isn't supported.

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

## parse_by_template {#template-options}

Parses the document by the user-generated template using customization options.

Learn more:
- https://docs.groupdocs.com/parser/python-net/parse-data-from-documents/
- https://docs.groupdocs.com/parser/python-net/working-with-templates/

```python
def parse_by_template(self, template, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| template | `Template` | The user-generated template. |
| options | `ParseByTemplateOptions` | The customization options. |

**Returns:** DocumentData | None: An instance of `DocumentData` that contains the extracted data; `None` if parsing by template isn't supported.

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

## parse_by_template {#template_collection-options}

Selects the most suitable template from the provided collection and then parses the document against the selected template.

```python
def parse_by_template(self, template_collection, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| template_collection | `TemplateCollection` | The template collection. |
| options | `ParseByTemplateOptions` | The customization options. |

**Returns:** DocumentData: An instance containing the extracted data, or None if parsing by template isn't supported.

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

### Aliases

These names call `parse_by_template` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `parse_by_template_template` | `parse_by_template_template(template, options)`<br>`parse_by_template_template(template)` |
| `parse_by_template_template_collection` | `parse_by_template_template_collection(template_collection, options)` |

### See Also
* class [`Parser`](/parser/python-net/groupdocs.parser/parser/)

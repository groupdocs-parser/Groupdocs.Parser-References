---
title: TemplateLinkedPosition class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Provides a template field position which uses the linked field."
type: docs
url: /python-net/groupdocs.parser.templates/templatelinkedposition/
is_root: false
weight: 70
---


## TemplateLinkedPosition class

Provides a template field position which uses the linked field.

The TemplateLinkedPosition type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.templates/templatelinkedposition/__init__/#linked_field_name-search_area-edges) | Initializes a new instance of the [`TemplateLinkedPosition`](/parser/python-net/groupdocs.parser.templates/templatelinkedposition/) class. |
| [__init__](/parser/python-net/groupdocs.parser.templates/templatelinkedposition/__init__/#linked_field_name-search_area-edges-auto_scale) | Initializes a new instance of TemplateLinkedPosition with an upper‑case linked field name. |
| [__init__](/parser/python-net/groupdocs.parser.templates/templatelinkedposition/__init__/#linked_field_name-search_area-edges-auto_scale-use_upper_case_name) | Initializes a new TemplateLinkedPosition instance. |

### Properties
| Property | Description |
| :- | :- |
| [auto_scale](/parser/python-net/groupdocs.parser.templates/templatelinkedposition/auto_scale/) | The value indicating whether the linked position's search area is scaled by the linked field size. |
| [edges](/parser/python-net/groupdocs.parser.templates/templatelinkedposition/edges/) | The edges of the linked field where a field is searched. |
| [linked_field_name](/parser/python-net/groupdocs.parser.templates/templatelinkedposition/linked_field_name/) | The linked field name as an uppercase string. |
| [search_area](/parser/python-net/groupdocs.parser.templates/templatelinkedposition/search_area/) | The size of the area where a field is searched. |

### Example

```python
from groupdocs.parser.data import Size
from groupdocs.parser.templates import (TemplateField, TemplateLinkedPosition,
                                        TemplateLinkedPositionEdges, TemplateRegexPosition)

# Create a regex template field to find "Invoice Number" text
invoice = TemplateField(TemplateRegexPosition("Invoice Number"), "Invoice")

# Create a related template field associated with "Invoice" field and extract the value on the right of it
invoice_number = TemplateField(
    TemplateLinkedPosition("invoice", Size(100, 15), TemplateLinkedPositionEdges(False, False, True, False)),
    "InvoiceNumber")
```

### See Also
* module [`groupdocs.parser.templates`](/parser/python-net/groupdocs.parser.templates/)

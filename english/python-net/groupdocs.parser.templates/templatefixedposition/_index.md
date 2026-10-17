---
title: TemplateFixedPosition class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Provides a template field position defined by a rectangular area."
type: docs
url: /python-net/groupdocs.parser.templates/templatefixedposition/
is_root: false
weight: 50
---


## TemplateFixedPosition class

Provides a template field position defined by a rectangular area.

This is the simplest way to define the field position. It requires setting a rectangular area on the page that bounds the field value. All the text that is contained (even partially) in the rectangular area will be extracted as a value:

```csharp
// Create a fixed template field with "Address" name which is bounded by a rectangle at the position (35, 160) and with the size (110, 20)
TemplateField templateField = new TemplateField(
    new TemplateFixedPosition(new Rectangle(new Point(35, 160), new Size(110, 20))),
    "Address");
```

The TemplateFixedPosition type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.templates/templatefixedposition/__init__/#rectangle) | Initializes a new instance of the TemplateFixedPosition class. |

### Properties
| Property | Description |
| :- | :- |
| [rectangle](/parser/python-net/groupdocs.parser.templates/templatefixedposition/rectangle/) | The rectangular area that contains the template field. |

### Example

```python
from groupdocs.parser.templates import TemplateFixedPosition, TemplateField, Template
from groupdocs.parser.data import Rectangle, Point, Size

field = TemplateField(
    TemplateFixedPosition(Rectangle(Point(35.0, 135.0), Size(100.0, 10.0))),
    "CompanyName",
)
```

### See Also
* module [`groupdocs.parser.templates`](/parser/python-net/groupdocs.parser.templates/)

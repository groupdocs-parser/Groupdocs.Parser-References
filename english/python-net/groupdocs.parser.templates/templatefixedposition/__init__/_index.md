---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new instance of the TemplateFixedPosition class."
type: docs
url: /python-net/groupdocs.parser.templates/templatefixedposition/__init__/
is_root: false
weight: 10
---


## __init__ {#rectangle}

Initializes a new instance of the TemplateFixedPosition class.

```python
def __init__(self, rectangle):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| rectangle | `Rectangle` | The rectangular area that contains the template field. |

### Example

```python
from groupdocs.parser.templates import TemplateFixedPosition
from groupdocs.parser.data import Rectangle, Point, Size

rect = Rectangle(Point(35.0, 135.0), Size(100.0, 10.0))
fixed_pos = TemplateFixedPosition(rect)
```

### See Also
* class [`TemplateFixedPosition`](/parser/python-net/groupdocs.parser.templates/templatefixedposition/)

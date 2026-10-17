---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new Point with the given coordinates."
type: docs
url: /python-net/groupdocs.parser.data/point/__init__/
is_root: false
weight: 10
---


## __init__ {#x-y}

Initializes a new [`Point`](/parser/python-net/groupdocs.parser.data/point/) with the given coordinates.

```python
def __init__(self, x, y):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| x | `float` | The x-coordinate. |
| y | `float` | The y-coordinate. |

### Example

```python
from groupdocs.parser.data import Point

p = Point(35.0, 135.0)
print(f"Point at ({p.x}, {p.y})")
```

### See Also
* class [`Point`](/parser/python-net/groupdocs.parser.data/point/)

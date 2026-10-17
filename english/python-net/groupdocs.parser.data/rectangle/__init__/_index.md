---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new Rectangle."
type: docs
url: /python-net/groupdocs.parser.data/rectangle/__init__/
is_root: false
weight: 10
---


## __init__ {#left-top-right-bottom}

Initializes a new Rectangle.

```python
def __init__(self, left, top, right, bottom):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| left | `float` | The x-coordinate of the left edge of the rectangular area. |
| top | `float` | The y-coordinate of the top edge of the rectangular area. |
| right | `float` | The x-coordinate of the right edge of the rectangular area. |
| bottom | `float` | The y-coordinate of the bottom edge of the rectangular area. |

## __init__ {#position-size}

Initializes a new Rectangle.

```python
def __init__(self, position, size):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| position | `Point` | The coordinates of the upper-left corner of the rectangular area. |
| size | `Size` | The size of the rectangular area. |

### Example

```python
from groupdocs.parser.data import Rectangle, Point, Size

rect = Rectangle(Point(35.0, 135.0), Size(100.0, 10.0))
```

### See Also
* class [`Rectangle`](/parser/python-net/groupdocs.parser.data/rectangle/)

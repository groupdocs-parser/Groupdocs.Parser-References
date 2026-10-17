---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new instance of the PageAreaOptions class."
type: docs
url: /python-net/groupdocs.parser.options/pageareaoptions/__init__/
is_root: false
weight: 10
---


## __init__

Initializes a new instance of the [`PageAreaOptions`](/parser/python-net/groupdocs.parser.options/pageareaoptions/) class.

```python
def __init__(self):
    ...
```

## __init__ {#rectangle}

Initializes a new instance of the PageAreaOptions class.

```python
def __init__(self, rectangle):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| rectangle | `Rectangle` | The rectangular area that contains page areas. |

### Example

```python
from groupdocs.parser.options import PageAreaOptions
from groupdocs.parser.data import Rectangle, Point, Size

rect = Rectangle(Point(0, 0), Size(100, 200))
options = PageAreaOptions(rect)
```

## __init__ {#rectangle-rectangle_tolerance}

Initializes a new instance of the PageAreaOptions class with the size of the ignored border.

```python
def __init__(self, rectangle, rectangle_tolerance):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| rectangle | `Rectangle` | The rectangular area that contains page areas. |
| rectangle_tolerance | `float` | The size of the border that is ignored when captured by the rectangular area. It's measured by the fraction of a text item height. |

### Example

```python
from groupdocs.parser.options import PageAreaOptions
from groupdocs.parser.data import Rectangle, Point, Size

# Define the area of interest on the page
rect = Rectangle(Point(0, 0), Size(500, 300))

# Create options with a tolerance of 0.1 (10% of text height)
options = PageAreaOptions(rect, rectangle_tolerance=0.1)
```

### See Also
* class [`PageAreaOptions`](/parser/python-net/groupdocs.parser.options/pageareaoptions/)

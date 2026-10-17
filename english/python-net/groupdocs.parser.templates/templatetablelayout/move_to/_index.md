---
title: move_to method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Creates a new layout with the same size, separators, and position at the specified point."
type: docs
url: /python-net/groupdocs.parser.templates/templatetablelayout/move_to/
is_root: false
weight: 1010
---


## move_to {#point}

Creates a new layout with the same size, separators, and position at the specified point.

This functionality allows moving a table layout. For documents where tables share the same column and row structure but appear at different positions, a [`TemplateTableLayout`](/parser/python-net/groupdocs.parser.templates/templatetablelayout/) can be defined once (e.g., at (0, 0)) and then moved to each table’s location. The method returns a copy of the original layout, so modifications to the moved layout do not affect the source layout. Any coordinates, including negative values, are accepted.

```python
def move_to(self, point):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| point | `Point` | The position of the new layout. |

**Returns:** A new layout with the same size, separators, and position at the specified point.

### Example

```python
from groupdocs.parser.data import Point
from groupdocs.parser.templates import TemplateTableLayout

# Create a table layout with column and row separators
layout = TemplateTableLayout(
    [0, 25, 150, 180, 230],
    [0, 15, 30, 45, 60, 75]
)

print(f"pos: ({layout.rectangle.left}, {layout.rectangle.top}) "
      f"size: ({layout.rectangle.size.width}, {layout.rectangle.size.height})")

# Move layout to a specific location
moved_layout = layout.move_to(Point(315, 250))

print(moved_layout.vertical_separators[0])   # 315
print(moved_layout.horizontal_separators[0]) # 250
```

### See Also
* class [`TemplateTableLayout`](/parser/python-net/groupdocs.parser.templates/templatetablelayout/)

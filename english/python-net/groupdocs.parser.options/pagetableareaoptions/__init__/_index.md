---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new PageAreaOptions instance."
type: docs
url: /python-net/groupdocs.parser.options/pagetableareaoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#table_layout}

Initializes a new PageAreaOptions instance.

```python
def __init__(self, table_layout):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| table_layout | `TemplateTableLayout` | The table layout which defines the table on a page. |

### Example

```python
from groupdocs.parser.options import PageTableAreaOptions
from groupdocs.parser.templates import TemplateTableLayout

# Define the layout of the table on the page
layout = TemplateTableLayout([50.0, 95.0, 275.0], [325.0, 340.0, 365.0])
# Create options with the custom layout
options = PageTableAreaOptions(layout)
```

### See Also
* class [`PageTableAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetableareaoptions/)

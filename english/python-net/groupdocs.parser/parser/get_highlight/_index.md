---
title: get_highlight method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Extracts a highlight from the document."
type: docs
url: /python-net/groupdocs.parser/parser/get_highlight/
is_root: false
weight: 1100
---


## get_highlight {#position-is_direct-options}

Extracts a highlight from the document.

Learn more:
- https://docs.groupdocs.com/parser/python-net/extract-highlights/

```python
def get_highlight(self, position, is_direct, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| position | `int` | The start position of the highlight. |
| is_direct | `bool` | True if the highlight is extracted to the right of `position`; otherwise False. |
| options | `HighlightOptions` | The highlight extraction options. |

**Returns:** HighlightItem: The extracted highlight; None if highlight extraction isn't supported.

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import HighlightOptions

with Parser("sample.docx") as parser:
    positions = [0, 100, 500, 1000]
    options = HighlightOptions(50)  # extract 50 characters
    for pos in positions:
        highlight = parser.get_highlight(pos, True, options)
        if highlight is not None:
            print(f"Position: {highlight.position}")
            print(f"Text: {highlight.text}")
```

### Aliases

These names call `get_highlight` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_highlight_int32` | `get_highlight_int32(position, is_direct, options)` |

### See Also
* class [`Parser`](/parser/python-net/groupdocs.parser/parser/)

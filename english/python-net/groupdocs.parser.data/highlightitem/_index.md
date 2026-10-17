---
title: HighlightItem class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Represents a highlight, a part of the text which is usually used to explain the context of the found text in the search functionality."
type: docs
url: /python-net/groupdocs.parser.data/highlightitem/
is_root: false
weight: 60
---


## HighlightItem class

Represents a highlight, a part of the text which is usually used to explain the context of the found text in the search functionality.

An instance of [`HighlightItem`](/parser/python-net/groupdocs.parser.data/highlightitem/) is used as the return value of [`Parser.get_highlight`](/parser/python-net/groupdocs.parser/parser/get_highlight/) (int, bool, [`HighlightOptions`](/parser/python-net/groupdocs.parser.options/highlightoptions/)) method, and of the [`SearchResult.left_highlight_item`](/parser/python-net/groupdocs.parser.data/searchresult/left_highlight_item/) and [`SearchResult.right_highlight_item`](/parser/python-net/groupdocs.parser.data/searchresult/right_highlight_item/) properties. See the usage examples there.

The HighlightItem type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [position](/parser/python-net/groupdocs.parser.data/highlightitem/position/) | The zero-based index of the start position of the highlight in the document text. |
| [text](/parser/python-net/groupdocs.parser.data/highlightitem/text/) | The text of the highlight. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import HighlightOptions

with Parser("./sample.pdf") as parser:
    options = HighlightOptions(20)  # extract 20 characters around the highlight
    highlight = parser.get_highlight(100, True, options)
    if highlight is not None:
        print(f"Position: {highlight.position}")
        print(f"Text: {highlight.text}")
```

### See Also
* module [`groupdocs.parser.data`](/parser/python-net/groupdocs.parser.data/)

---
title: SearchResult class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Represents the search result in the search functionality."
type: docs
url: /python-net/groupdocs.parser.data/searchresult/
is_root: false
weight: 190
---


## SearchResult class

Represents the search result in the search functionality.

An instance of [`SearchResult`](/parser/python-net/groupdocs.parser.data/searchresult/) class is used as return value of [`Parser.search`](/parser/python-net/groupdocs.parser/parser/search/) and [`Parser.search`](/parser/python-net/groupdocs.parser/parser/search/) methods. See the usage examples there.

The SearchResult type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [left_highlight_item](/parser/python-net/groupdocs.parser.data/searchresult/left_highlight_item/) | The left highlight item. |
| [page_index](/parser/python-net/groupdocs.parser.data/searchresult/page_index/) | The page index where the text is found. Zero-based index of the page where the text is found; None if the search is performed on the whole document text. |
| [position](/parser/python-net/groupdocs.parser.data/searchresult/position/) | The position in the document text. |
| [right_highlight_item](/parser/python-net/groupdocs.parser.data/searchresult/right_highlight_item/) | The right highlight item. |
| [text](/parser/python-net/groupdocs.parser.data/searchresult/text/) | The text of the search result. |

### Example

```python
from groupdocs.parser import Parser

with Parser("./sample.pdf") as parser:
    search_results = parser.search("lorem")
    if search_results is None:
        print("Search isn't supported")
    else:
        for result in search_results:
            print(f"At {result.position}: {result.text}")
```

### See Also
* module [`groupdocs.parser.data`](/parser/python-net/groupdocs.parser.data/)

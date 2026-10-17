---
title: SearchOptions class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Provides the options which are used for text search."
type: docs
url: /python-net/groupdocs.parser.options/searchoptions/
is_root: false
weight: 420
---


## SearchOptions class

Provides the options which are used for text search.

An instance of [`SearchOptions`](/parser/python-net/groupdocs.parser.options/searchoptions/) class is used as a parameter in [`Parser.search`](/parser/python-net/groupdocs.parser/parser/search/) method. See the usage examples there.

The SearchOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.options/searchoptions/__init__/#match_case-match_whole_word-use_regular_expression-search_by_pages-left_highlight_options-right_highlight_options) | Initializes a new instance of the SearchOptions class. |
| [__init__](/parser/python-net/groupdocs.parser.options/searchoptions/__init__/#match_case-match_whole_word-use_regular_expression-max_page_index-left_highlight_options-right_highlight_options) | Initializes a new instance of the [`SearchOptions`](/parser/python-net/groupdocs.parser.options/searchoptions/) class with the page limit. |
| [__init__](/parser/python-net/groupdocs.parser.options/searchoptions/__init__/#match_case-match_whole_word-use_regular_expression-left_highlight_options-right_highlight_options) | Initializes a new instance of the SearchOptions class which is used to search with the highlight options for the left and the right highlight extraction. |
| [__init__](/parser/python-net/groupdocs.parser.options/searchoptions/__init__/#match_case-match_whole_word-use_regular_expression-highlight_options) | Initializes a new instance of the SearchOptions class which is used to search with the same highlight options for the left and the right highlight extraction. |
| [__init__](/parser/python-net/groupdocs.parser.options/searchoptions/__init__/#match_case-match_whole_word-use_regular_expression) | Initializes a new SearchOptions instance used to search without highlight extraction. |
| [__init__](/parser/python-net/groupdocs.parser.options/searchoptions/__init__/#match_case-match_whole_word-use_regular_expression-search_by_pages) | Initializes a new SearchOptions instance used to search by pages without highlight extraction. |
| [__init__](/parser/python-net/groupdocs.parser.options/searchoptions/__init__/) | Initializes a new instance of the SearchOptions class with default values. |

### Properties
| Property | Description |
| :- | :- |
| [left_highlight_options](/parser/python-net/groupdocs.parser.options/searchoptions/left_highlight_options/) | The options for the left highlight. |
| [match_case](/parser/python-net/groupdocs.parser.options/searchoptions/match_case/) | The value indicates whether text case is considered (i.e., not ignored) during a search. |
| [match_whole_word](/parser/python-net/groupdocs.parser.options/searchoptions/match_whole_word/) | The value indicates whether text search is limited by a whole word. |
| [max_page_index](/parser/python-net/groupdocs.parser.options/searchoptions/max_page_index/) | The max page index to search; -1 indicates not set. |
| [right_highlight_options](/parser/python-net/groupdocs.parser.options/searchoptions/right_highlight_options/) | The options for the right highlight. |
| [search_by_pages](/parser/python-net/groupdocs.parser.options/searchoptions/search_by_pages/) | The value indicating whether the search is performed by pages. |
| [use_regular_expression](/parser/python-net/groupdocs.parser.options/searchoptions/use_regular_expression/) | The value indicating whether a regular expression is used. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import SearchOptions

with Parser("sample.pdf") as parser:
    # match_case, match_whole_word, use_regular_expression, search_by_pages
    options = SearchOptions(False, False, False, True)
    results = parser.search("lorem", options)
    if results is None:
        print("Search isn't supported for this format.")
    else:
        for result in results:
            print(f"Found on page {result.page_index + 1}: {result.text}")
```

### See Also
* module [`groupdocs.parser.options`](/parser/python-net/groupdocs.parser.options/)

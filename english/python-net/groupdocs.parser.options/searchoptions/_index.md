---
title: SearchOptions class
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.options/searchoptions/
is_root: false
weight: 340
---

## SearchOptions class

Provides the options which are used for text search.



The SearchOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.options/searchoptions/__init__/#bool-bool-bool-bool-groupdocs.parser.options.HighlightOptions-groupdocs.parser.options.HighlightOptions) | Initializes a new instance of the [`SearchOptions`](/parser/python-net/groupdocs.parser.options/searchoptions) class. |
| [__init__](/parser/python-net/groupdocs.parser.options/searchoptions/__init__/#bool-bool-bool-int-groupdocs.parser.options.HighlightOptions-groupdocs.parser.options.HighlightOptions) | Initializes a new instance of the [`SearchOptions`](/parser/python-net/groupdocs.parser.options/searchoptions) class with the page limit. |
| [__init__](/parser/python-net/groupdocs.parser.options/searchoptions/__init__/#bool-bool-bool-groupdocs.parser.options.HighlightOptions-groupdocs.parser.options.HighlightOptions) | Initializes a new instance of the [`SearchOptions`](/parser/python-net/groupdocs.parser.options/searchoptions) class which is used to search<br/>with the highlight options for the left and the right highlight extraction. |
| [__init__](/parser/python-net/groupdocs.parser.options/searchoptions/__init__/#bool-bool-bool-groupdocs.parser.options.HighlightOptions) | Initializes a new instance of the [`SearchOptions`](/parser/python-net/groupdocs.parser.options/searchoptions) class which is used to search<br/>with the same highlight options for the left and the right highlight extraction. |
| [__init__](/parser/python-net/groupdocs.parser.options/searchoptions/__init__/#bool-bool-bool) | Initializes a new instance of the [`SearchOptions`](/parser/python-net/groupdocs.parser.options/searchoptions) class which is used to search<br/>without highlight extraction. |
| [__init__](/parser/python-net/groupdocs.parser.options/searchoptions/__init__/#bool-bool-bool-bool) | Initializes a new instance of the [`SearchOptions`](/parser/python-net/groupdocs.parser.options/searchoptions) class which is used to search by pages and<br/>without highlight extraction. |
| [__init__](/parser/python-net/groupdocs.parser.options/searchoptions/__init__/#) | Initializes a new instance of the [`SearchOptions`](/parser/python-net/groupdocs.parser.options/searchoptions) class with default values. See remarks for details. |


### Properties
| Property | Description |
| :- | :- |
| [match_case](/parser/python-net/groupdocs.parser.options/searchoptions/match_case) | Gets the value that indicates whether a text case isn't ignored. |
| [match_whole_word](/parser/python-net/groupdocs.parser.options/searchoptions/match_whole_word) | Gets the value that indicates whether text search is limited by a whole word. |
| [use_regular_expression](/parser/python-net/groupdocs.parser.options/searchoptions/use_regular_expression) | Gets the value that indicates whether a regular expression is used. |
| [search_by_pages](/parser/python-net/groupdocs.parser.options/searchoptions/search_by_pages) | Gets the value that indicates whether the search is performed by pages. |
| [max_page_index](/parser/python-net/groupdocs.parser.options/searchoptions/max_page_index) | Gets the value that represents the max index of the page to search. |
| [left_highlight_options](/parser/python-net/groupdocs.parser.options/searchoptions/left_highlight_options) | Gets the options for the left highlight. |
| [right_highlight_options](/parser/python-net/groupdocs.parser.options/searchoptions/right_highlight_options) | Gets the options for the right highlight. |



### Remarks 


An instance of [`SearchOptions`](/parser/python-net/groupdocs.parser.options/searchoptions) class is used as parameter 
in [`Parser.search`](/parser/python-net/groupdocs.parser/parser/search) method. See the usage examples there.

### See Also
* module [`groupdocs.parser.options`](..)
* class [`SearchOptions`](/parser/python-net/groupdocs.parser.options/searchoptions)

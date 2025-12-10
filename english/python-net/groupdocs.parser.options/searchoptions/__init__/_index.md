---
title: SearchOptions constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.options/searchoptions/__init__/
is_root: false
weight: 10
---

## __init__ {#}

Initializes a new instance of the [`SearchOptions`](/parser/python-net/groupdocs.parser.options/searchoptions) class with default values. See remarks for details.



```python
def __init__(self):
    ...
```




## __init__ {#bool-bool-bool}

Initializes a new instance of the [`SearchOptions`](/parser/python-net/groupdocs.parser.options/searchoptions) class which is used to search
without highlight extraction.



```python
def __init__(self, match_case, match_whole_word, use_regular_expression):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| match_case | bool | The value that indicates whether a text case isn't ignored. |
| match_whole_word | bool | The value that indicates whether text search is limited by a whole word. |
| use_regular_expression | bool | The value that indicates whether a regular expression is used. |


## __init__ {#bool-bool-bool-groupdocs.parser.options.HighlightOptions}

Initializes a new instance of the [`SearchOptions`](/parser/python-net/groupdocs.parser.options/searchoptions) class which is used to search
with the same highlight options for the left and the right highlight extraction.



```python
def __init__(self, match_case, match_whole_word, use_regular_expression, highlight_options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| match_case | bool | The value that indicates whether a text case isn't ignored. |
| match_whole_word | bool | The value that indicates whether text search is limited by a whole word. |
| use_regular_expression | bool | The value that indicates whether a regular expression is used. |
| highlight_options | groupdocs.parser.options.HighlightOptions | The options for both highlights. |


## __init__ {#bool-bool-bool-bool}

Initializes a new instance of the [`SearchOptions`](/parser/python-net/groupdocs.parser.options/searchoptions) class which is used to search by pages and
without highlight extraction.



```python
def __init__(self, match_case, match_whole_word, use_regular_expression, search_by_pages):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| match_case | bool | The value that indicates whether a text case isn't ignored. |
| match_whole_word | bool | The value that indicates whether text search is limited by a whole word. |
| use_regular_expression | bool | The value that indicates whether a regular expression is used. |
| search_by_pages | bool | The value that indicates whether the search is performed by pages. |


## __init__ {#bool-bool-bool-groupdocs.parser.options.HighlightOptions-groupdocs.parser.options.HighlightOptions}

Initializes a new instance of the [`SearchOptions`](/parser/python-net/groupdocs.parser.options/searchoptions) class which is used to search
with the highlight options for the left and the right highlight extraction.



```python
def __init__(self, match_case, match_whole_word, use_regular_expression, left_highlight_options, right_highlight_options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| match_case | bool | The value that indicates whether a text case isn't ignored. |
| match_whole_word | bool | The value that indicates whether text search is limited by a whole word. |
| use_regular_expression | bool | The value that indicates whether a regular expression is used. |
| left_highlight_options | groupdocs.parser.options.HighlightOptions | The options for the left highlight. |
| right_highlight_options | groupdocs.parser.options.HighlightOptions | The options for the right highlight. |


## __init__ {#bool-bool-bool-bool-groupdocs.parser.options.HighlightOptions-groupdocs.parser.options.HighlightOptions}

Initializes a new instance of the [`SearchOptions`](/parser/python-net/groupdocs.parser.options/searchoptions) class.



```python
def __init__(self, match_case, match_whole_word, use_regular_expression, search_by_pages, left_highlight_options, right_highlight_options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| match_case | bool | The value that indicates whether a text case isn't ignored. |
| match_whole_word | bool | The value that indicates whether text search is limited by a whole word. |
| use_regular_expression | bool | The value that indicates whether a regular expression is used. |
| search_by_pages | bool | The value that indicates whether the search is performed by pages. |
| left_highlight_options | groupdocs.parser.options.HighlightOptions | The options for the left highlight. |
| right_highlight_options | groupdocs.parser.options.HighlightOptions | The options for the right highlight. |


## __init__ {#bool-bool-bool-int-groupdocs.parser.options.HighlightOptions-groupdocs.parser.options.HighlightOptions}

Initializes a new instance of the [`SearchOptions`](/parser/python-net/groupdocs.parser.options/searchoptions) class with the page limit.



```python
def __init__(self, match_case, match_whole_word, use_regular_expression, max_page_index, left_highlight_options, right_highlight_options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| match_case | bool | The value that indicates whether a text case isn't ignored. |
| match_whole_word | bool | The value that indicates whether text search is limited by a whole word. |
| use_regular_expression | bool | The value that indicates whether a regular expression is used. |
| max_page_index | int | he value that indicates whether the search is performed by pages. |
| left_highlight_options | groupdocs.parser.options.HighlightOptions | The options for the left highlight. |
| right_highlight_options | groupdocs.parser.options.HighlightOptions | The options for the right highlight. |



### See Also
* module [`groupdocs.parser.options`](../../)
* class [`SearchOptions`](/parser/python-net/groupdocs.parser.options/searchoptions)

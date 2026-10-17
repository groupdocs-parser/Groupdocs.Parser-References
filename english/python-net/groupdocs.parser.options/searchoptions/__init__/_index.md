---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new instance of the SearchOptions class."
type: docs
url: /python-net/groupdocs.parser.options/searchoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#match_case-match_whole_word-use_regular_expression-search_by_pages-left_highlight_options-right_highlight_options}

Initializes a new instance of the SearchOptions class.

```python
def __init__(self, match_case, match_whole_word, use_regular_expression, search_by_pages, left_highlight_options, right_highlight_options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| match_case | `bool` | Indicates whether text case is considered. |
| match_whole_word | `bool` | Indicates whether the search is limited to whole words. |
| use_regular_expression | `bool` | Indicates whether a regular expression is used. |
| search_by_pages | `bool` | Indicates whether the search is performed by pages. |
| left_highlight_options | `HighlightOptions` | The options for the left highlight. |
| right_highlight_options | `HighlightOptions` | The options for the right highlight. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import SearchOptions

with Parser("sample.pdf") as parser:
    options = SearchOptions(False, False, False, True)
    results = parser.search("lorem", options)
    if results is None:
        print("Search isn't supported for this format.")
    else:
        for result in results:
            print(f"Found on page {result.page_index + 1}: {result.text}")
```

## __init__ {#match_case-match_whole_word-use_regular_expression-max_page_index-left_highlight_options-right_highlight_options}

Initializes a new instance of the [`SearchOptions`](/parser/python-net/groupdocs.parser.options/searchoptions/) class with the page limit.

```python
def __init__(self, match_case, match_whole_word, use_regular_expression, max_page_index, left_highlight_options, right_highlight_options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| match_case | `bool` | The value that indicates whether a text case isn't ignored. |
| match_whole_word | `bool` | The value that indicates whether text search is limited by a whole word. |
| use_regular_expression | `bool` | The value that indicates whether a regular expression is used. |
| max_page_index | `int` | The value that indicates whether the search is performed by pages. |
| left_highlight_options | `HighlightOptions` | The options for the left highlight. |
| right_highlight_options | `HighlightOptions` | The options for the right highlight. |

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

## __init__ {#match_case-match_whole_word-use_regular_expression-left_highlight_options-right_highlight_options}

Initializes a new instance of the SearchOptions class which is used to search with the highlight options for the left and the right highlight extraction.

```python
def __init__(self, match_case, match_whole_word, use_regular_expression, left_highlight_options, right_highlight_options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| match_case | `bool` | The value that indicates whether a text case isn't ignored. |
| match_whole_word | `bool` | The value that indicates whether text search is limited by a whole word. |
| use_regular_expression | `bool` | The value that indicates whether a regular expression is used. |
| left_highlight_options | `HighlightOptions` | The options for the left highlight. |
| right_highlight_options | `HighlightOptions` | The options for the right highlight. |

## __init__ {#match_case-match_whole_word-use_regular_expression-highlight_options}

Initializes a new instance of the SearchOptions class which is used to search with the same highlight options for the left and the right highlight extraction.

```python
def __init__(self, match_case, match_whole_word, use_regular_expression, highlight_options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| match_case | `bool` | Indicates whether text case is not ignored. |
| match_whole_word | `bool` | Indicates whether text search is limited by a whole word. |
| use_regular_expression | `bool` | Indicates whether a regular expression is used. |
| highlight_options | `HighlightOptions` | Options for both highlights. |

### Example

```python
    from groupdocs.parser import Parser
    from groupdocs.parser.options import SearchOptions

    with Parser("sample.pdf") as parser:
        # match_case, match_whole_word, use_regular_expression, highlight_options
        options = SearchOptions(False, False, False, True)
        results = parser.search("lorem", options)
        if results is None:
            print("Search isn't supported for this format.")
        else:
            for result in results:
                print(f"Found on page {result.page_index + 1}: {result.text}")
    ```

## __init__ {#match_case-match_whole_word-use_regular_expression}

Initializes a new SearchOptions instance used to search without highlight extraction.

```python
def __init__(self, match_case, match_whole_word, use_regular_expression):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| match_case | `bool` | Indicates whether text case is not ignored (i.e., case‑sensitive search). |
| match_whole_word | `bool` | Indicates whether the search is limited to whole words. |
| use_regular_expression | `bool` | Indicates whether a regular expression is used for the search. |

## __init__ {#match_case-match_whole_word-use_regular_expression-search_by_pages}

Initializes a new SearchOptions instance used to search by pages without highlight extraction.

```python
def __init__(self, match_case, match_whole_word, use_regular_expression, search_by_pages):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| match_case | `bool` | Indicates whether text case is not ignored. |
| match_whole_word | `bool` | Indicates whether text search is limited to whole words. |
| use_regular_expression | `bool` | Indicates whether a regular expression is used. |
| search_by_pages | `bool` | Indicates whether the search is performed by pages. |

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

## __init__

Initializes a new instance of the SearchOptions class with default values.

The following properties have default values:

- `MatchCase`: False
- `MatchWholeWord`: False
- `UseRegularExpression`: False
- `LeftHighlightOptions`: None
- `RightHighlightOptions`: None

```python
def __init__(self):
    ...
```

### See Also
* class [`SearchOptions`](/parser/python-net/groupdocs.parser.options/searchoptions/)

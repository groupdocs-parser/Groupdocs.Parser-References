---
title: search method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Searches a keyword in the document."
type: docs
url: /python-net/groupdocs.parser/parser/search/
is_root: false
weight: 1250
---


## search {#keyword}

Searches a keyword in the document.

Learn more:
- [Search text](https://docs.groupdocs.com/parser/python-net/search-text/)

```python
def search(self, keyword):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| keyword | `str` | The keyword to search. |

**Returns:** Iterable[SearchResult] | None: A collection of search result objects; None if search isn't supported.

### Example

```python
from groupdocs.parser import Parser

with Parser("sample.pdf") as parser:
    results = parser.search("lorem")
    if results is None:
        print("Search isn't supported for this format.")
    else:
        for result in results:
            print(f"Found at {result.position}: {result.text}")
```

## search {#keyword-options}

Searches a keyword in the document using search options (regular expression, match case, etc.).

```python
def search(self, keyword, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| keyword | `str` | The keyword to search. |
| options | `SearchOptions` | The search options. |

**Returns:** Iterable[SearchResult] or None: A collection of `SearchResult` objects; `None` if search isn't supported.

Remarks:
- [Search text](https://docs.groupdocs.com/parser/python-net/search-text/)

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

### Aliases

These names call `search` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `search_file` | `search_file(keyword, options)`<br>`search_file(keyword)` |
| `search_string` | `search_string(keyword, options)`<br>`search_string(keyword)` |

### See Also
* class [`Parser`](/parser/python-net/groupdocs.parser/parser/)

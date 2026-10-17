---
title: search method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Searches a keyword in the document."
type: docs
url: /python-net/groupdocs.parser/parser/search/
is_root: false
weight: 1540
---


## search {#keyword}

Searches a keyword in the document.

Learn more:
- [Search text](https://docs.groupdocs.com/display/parsernet/Search+text)
- [Search text in Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
- [Search text in Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
- [Search text in Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
- [Search text in PDF documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
- [Search text in Emails](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
- [Search text in EPUB eBooks](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
- [Search text in HTML documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
- [Search text in Microsoft OneNote sections](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

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
- [Search text](https://docs.groupdocs.com/display/parsernet/Search+text)
- [Search text in Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
- [Search text in Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
- [Search text in Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
- [Search text in PDF documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
- [Search text in Emails](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
- [Search text in EPUB eBooks](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
- [Search text in HTML documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
- [Search text in Microsoft OneNote sections](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

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

### See Also
* class [`Parser`](/parser/python-net/groupdocs.parser/parser/)

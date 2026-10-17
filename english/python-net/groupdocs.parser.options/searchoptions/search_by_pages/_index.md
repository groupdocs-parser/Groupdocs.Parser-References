---
title: search_by_pages property
second_title: GroupDocs.Parser for Python via .NET API References
description: "The value indicating whether the search is performed by pages."
type: docs
url: /python-net/groupdocs.parser.options/searchoptions/search_by_pages/
is_root: false
weight: 2060
---


## search_by_pages property

The value indicating whether the search is performed by pages.

True if the search is performed by pages; otherwise False and the search is performed on the whole document without including [`SearchResult.PageIndex`](/parser/python-net/groupdocs.parser.data/searchresult/page_index/) property value in [`SearchResult`](/parser/python-net/groupdocs.parser.data/searchresult/) class.

### Definition:
```python
@property
def search_by_pages(self):
    ...
@search_by_pages.setter
def search_by_pages(self, value):
    ...
```

### See Also
* class [`SearchOptions`](/parser/python-net/groupdocs.parser.options/searchoptions/)

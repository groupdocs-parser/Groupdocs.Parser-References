---
title: get_toc method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Extracts a table of contents from the document."
type: docs
url: /python-net/groupdocs.parser/parser/get_toc/
is_root: false
weight: 1430
---


## get_toc

Extracts a table of contents from the document.

Learn more:
- https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents
- https://docs.groupdocs.com/display/parsernet/Extract+text+by+table+of+contents+item
- https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents+from+Microsoft+Office+Word+documents
- https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents+from+EPUB+eBooks

```python
def get_toc(self):
    ...
```

**Returns:** Iterable[TocItem] – collection of table of contents items; None if table of contents extraction isn't supported.

### Example

```python
from groupdocs.parser import Parser

# Initialize parser with the path to the document
with Parser(file_path) as parser:
    # Verify that text extraction is supported
    if not parser.features.text:
        print("Text extraction isn't supported.")
        exit()

    # Verify that TOC extraction is supported
    if not parser.features.toc:
        print("TOC extraction isn't supported.")
        exit()

    # Get table of contents
    toc = parser.get_toc()
    if toc is None:
        print("TOC extraction not supported for this document.")
    else:
        for item in toc:
            print(item.text)
            if item.page_index is not None:
                # Extract text for the page referenced by the TOC item
                page_text = parser.get_text(item.page_index)
                print(page_text)
```

### See Also
* class [`Parser`](/parser/python-net/groupdocs.parser/parser/)

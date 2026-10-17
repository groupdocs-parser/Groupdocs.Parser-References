---
title: get_hyperlinks method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Extracts hyperlinks from the document."
type: docs
url: /python-net/groupdocs.parser/parser/get_hyperlinks/
is_root: false
weight: 1240
---


## get_hyperlinks

Extracts hyperlinks from the document.

```python
def get_hyperlinks(self):
    ...
```

**Returns:** Iterable[PageHyperlinkArea] or None: A collection of `PageHyperlinkArea` objects, or `None` if hyperlink extraction isn't supported.

### Example

```python
from groupdocs.parser import Parser

with Parser("document.pdf") as parser:
    if not parser.features.hyperlinks:
        print("Hyperlink extraction not supported")
    else:
        hyperlinks = parser.get_hyperlinks()
        if hyperlinks:
            for hyperlink in hyperlinks:
                print(hyperlink.text)
                print(hyperlink.url)
                print()
```

## get_hyperlinks {#page_index}

Extracts hyperlinks from the document page.

```python
def get_hyperlinks(self, page_index):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| page_index | `int` | The zero-based page index. |

**Returns:** Iterable[PageHyperlinkArea] | None: A collection of PageHyperlinkArea objects, or None if hyperlink extraction isn't supported.

### Example

```python
from groupdocs.parser import Parser

with Parser("./document.pdf") as parser:
    # Verify that the document supports hyperlink extraction
    if not parser.features.hyperlinks:
        print("Hyperlink extraction not supported")
    else:
        page_index = 0
        hyperlinks = parser.get_hyperlinks(page_index)
        if hyperlinks:
            for link in hyperlinks:
                print(f"Text: {link.text}, URL: {link.url}")
```

## get_hyperlinks {#options}

Extracts hyperlinks from the document using customization options (to set the rectangular area that contains hyperlinks).

```python
def get_hyperlinks(self, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| options | `PageAreaOptions` | The options for hyperlinks extraction. |

**Returns:** list[PageHyperlinkArea] or None: A collection of PageHyperlinkArea objects; None if hyperlink extraction isn't supported.

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.data import Rectangle, Point, Size
from groupdocs.parser.options import PageAreaOptions

with Parser("file.pdf") as parser:
    if not parser.features.hyperlinks:
        print("Hyperlink extraction not supported")
    else:
        # Define the rectangular area that contains hyperlinks
        options = PageAreaOptions(Rectangle(Point(380, 90), Size(150, 50)))
        hyperlinks = parser.get_hyperlinks(options)
        for link in hyperlinks:
            print(link.text)
            print(link.url)
```

## get_hyperlinks {#page_index-options}

Extracts hyperlinks from the document page using customization options to set the rectangular area that contains hyperlinks.

```python
def get_hyperlinks(self, page_index, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| page_index | `int` | The zero‑based page index. |
| options | `PageAreaOptions` | The options for hyperlinks extraction. |

**Returns:** Iterable[PageHyperlinkArea] | None: A collection of `PageHyperlinkArea` objects; `None` if hyperlink extraction isn't supported.

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.data import Rectangle, Point, Size
from groupdocs.parser.options import PageAreaOptions

file_path = "sample.pdf"
with Parser(file_path) as parser:
    if not parser.features.hyperlinks:
        print("Document doesn't support hyperlink extraction")
        exit()

    doc_info = parser.get_document_info()
    if doc_info.page_count == 0:
        print("Document has no pages")
        exit()

    # Define the area that contains hyperlinks
    options = PageAreaOptions(Rectangle(Point(380, 90), Size(150, 50)))

    for page_index in range(doc_info.page_count):
        print(f"Page {page_index + 1}/{doc_info.page_count}")
        hyperlinks = parser.get_hyperlinks(page_index, options)
        if not hyperlinks:
            continue
        for h in hyperlinks:
            print(h.text)
            print(h.url)
            print()
```

### See Also
* class [`Parser`](/parser/python-net/groupdocs.parser/parser/)

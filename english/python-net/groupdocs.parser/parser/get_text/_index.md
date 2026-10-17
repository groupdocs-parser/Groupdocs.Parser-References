---
title: get_text method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Extracts text from the document."
type: docs
url: /python-net/groupdocs.parser/parser/get_text/
is_root: false
weight: 1370
---


## get_text

Extracts text from the document.

Learn more:
- [Extract text from documents](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
- [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

```python
def get_text(self):
    ...
```

**Returns:** io.TextIOBase: An instance with the extracted text, or None if text extraction isn't supported.

### Example

```python
from groupdocs.parser import Parser

with Parser("./sample.pdf") as parser:
    text_reader = parser.get_text()
    if text_reader is not None:
        print(text_reader.read_to_end())
```

## get_text {#options}

Extracts a text page from the document using text options (to enable raw fast text extraction mode).

Learn more:
- https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode
- https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode

```python
def get_text(self, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| options | `TextOptions` | The text extraction options. |

**Returns:** An instance of `io.TextIOBase` with the extracted text; `None` if text extraction isn't supported.

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import TextOptions

with Parser("./sample.pdf") as parser:
    # Enable raw fast text extraction mode
    options = TextOptions(True)  # raw fast mode
    text_reader = parser.get_text(options)
    if text_reader is not None:
        print(text_reader.read_to_end())
```

## get_text {#page_index}

Extracts text from a specific page of the document.

The method returns a `TextReader` containing the extracted text, or `None` if text extraction for the page is not supported.

```python
def get_text(self, page_index):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| page_index | `int` | The zero‑based page index. |

**Returns:** TextReader | None: A `TextReader` with the extracted text, or `None` if the page cannot be extracted.

Remarks:
- Learn more: https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode

### Example

```python
from groupdocs.parser import Parser

with Parser("./sample.pdf") as parser:
    # Extract text from the first page (page index 0)
    reader = parser.get_text(0)
    if reader is not None:
        print(reader.read_to_end())
```

## get_text {#page_index-options}

Extracts text from a specific page of the document using text options (enables raw fast text extraction mode).

```python
def get_text(self, page_index, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| page_index | `int` | The zero‑based page index. |
| options | `TextOptions` | The text extraction options. |

**Returns:** io.TextIOBase: A text reader with the extracted text, or None if text extraction for the page is not supported.

Learn more:
- https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode
- https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import TextOptions

with Parser("./sample.pdf") as parser:
    # Ensure the document supports text extraction
    if not parser.features.text:
        print("Document does not support text extraction.")
    else:
        # Extract raw text from the first page
        reader = parser.get_text(0, TextOptions(True))
        if reader is not None:
            print(reader.read_to_end())
```

### See Also
* class [`Parser`](/parser/python-net/groupdocs.parser/parser/)

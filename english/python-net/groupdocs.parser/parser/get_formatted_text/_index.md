---
title: get_formatted_text method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Extracts formatted text from the document."
type: docs
url: /python-net/groupdocs.parser/parser/get_formatted_text/
is_root: false
weight: 1090
---


## get_formatted_text {#options}

Extracts formatted text from the document.

```python
def get_formatted_text(self, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| options | `FormattedTextOptions` | The formatted text extraction options. |

**Returns:** System.IO.TextReader or None: An instance of `System.IO.TextReader` class with the extracted text; `None` if formatted text extraction isn't supported.

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import FormattedTextOptions, FormattedTextMode

with Parser("sample.pptx") as parser:
    reader = parser.get_formatted_text(FormattedTextOptions(FormattedTextMode.MARKDOWN))
    print(reader.read_to_end() if reader is not None else "Formatted text isn't available.")
```

## get_formatted_text {#page_index-options}

Extracts formatted text from a document page.

Learn more:
- Extract a document text as HTML
- Extract a document text as Markdown
- Extract a document text as Plain text

```python
def get_formatted_text(self, page_index, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| page_index | `int` | The zero‑based page index. |
| options | `FormattedTextOptions` | The formatted text extraction options. |

**Returns:** io.TextIOBase or None: A text reader with the extracted text; `None` if formatted text page extraction isn't supported.

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import FormattedTextOptions, FormattedTextMode

with Parser("sample.pptx") as parser:
    # Extract formatted text from the first page as Markdown
    reader = parser.get_formatted_text(0, FormattedTextOptions(FormattedTextMode.MARKDOWN))
    if reader is not None:
        print(reader.read_to_end())
    else:
        print("Formatted text isn't available.")
```

### Aliases

These names call `get_formatted_text` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_formatted_text_int32` | `get_formatted_text_int32(page_index, options)` |
| `get_formatted_text_formatted_text_options` | `get_formatted_text_formatted_text_options(options)` |

### See Also
* class [`Parser`](/parser/python-net/groupdocs.parser/parser/)

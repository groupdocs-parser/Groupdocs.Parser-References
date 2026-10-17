---
title: get_formatted_text method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Extracts formatted text from the document."
type: docs
url: /python-net/groupdocs.parser/parser/get_formatted_text/
is_root: false
weight: 1190
---


## get_formatted_text {#options}

Extracts formatted text from the document.

Learn more:

- [Extract formatted text from document](https://docs.groupdocs.com/display/parsernet/Extract+formatted+text+from+document)
- [Extract a document text as HTML](https://docs.groupdocs.com/display/parsernet/HTML)
- [Extract a document text as Markdown](https://docs.groupdocs.com/display/parsernet/Markdown)
- [Extract a document text as Plain text](https://docs.groupdocs.com/display/parsernet/Plain+text)

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
- [Extract formatted text from document page](https://docs.groupdocs.com/display/parsernet/Extract+formatted+text+from+document+page)
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

### See Also
* class [`Parser`](/parser/python-net/groupdocs.parser/parser/)

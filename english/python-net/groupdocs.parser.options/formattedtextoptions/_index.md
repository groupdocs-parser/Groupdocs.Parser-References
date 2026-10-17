---
title: FormattedTextOptions class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Provides the options which are used for formatted text extraction."
type: docs
url: /python-net/groupdocs.parser.options/formattedtextoptions/
is_root: false
weight: 170
---


## FormattedTextOptions class

Provides the options which are used for formatted text extraction.

An instance of [`FormattedTextOptions`](/parser/python-net/groupdocs.parser.options/formattedtextoptions/) is used as a parameter in [`Parser.get_formatted_text`](/parser/python-net/groupdocs.parser/parser/get_formatted_text/) and [`Parser.get_formatted_text`](/parser/python-net/groupdocs.parser/parser/get_formatted_text/) methods. See the usage examples there.

- Extract formatted text from document
- Extract a document text as HTML
- Extract a document text as Markdown
- Extract a document text as Plain text

The FormattedTextOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.options/formattedtextoptions/__init__/) | Initializes a new instance of the [`FormattedTextOptions`](/parser/python-net/groupdocs.parser.options/formattedtextoptions/) class. |
| [__init__](/parser/python-net/groupdocs.parser.options/formattedtextoptions/__init__/#mode) | Initializes a new FormattedTextOptions instance. |

### Properties
| Property | Description |
| :- | :- |
| [mode](/parser/python-net/groupdocs.parser.options/formattedtextoptions/mode/) | The formatted text extraction mode. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import FormattedTextOptions, FormattedTextMode

with Parser("sample.pptx") as parser:
    # Extract formatted text as Markdown (HTML and PLAIN_TEXT modes are also available)
    reader = parser.get_formatted_text(FormattedTextOptions(FormattedTextMode.MARKDOWN))
    print(reader.read_to_end() if reader is not None else "Formatted text isn't available.")
```

### See Also
* module [`groupdocs.parser.options`](/parser/python-net/groupdocs.parser.options/)

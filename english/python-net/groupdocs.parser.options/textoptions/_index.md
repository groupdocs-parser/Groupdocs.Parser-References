---
title: TextOptions class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Provides the options which are used for text extraction."
type: docs
url: /python-net/groupdocs.parser.options/textoptions/
is_root: false
weight: 440
---


## TextOptions class

Provides the options which are used for text extraction.

An instance of [`TextOptions`](/parser/python-net/groupdocs.parser.options/textoptions/) is used as a parameter in [`Parser.get_text`](/parser/python-net/groupdocs.parser/parser/get_text/) and [`Parser.get_text`](/parser/python-net/groupdocs.parser/parser/get_text/) methods. See the usage examples there.

It specifies the raw mode of text extraction. Text in this mode is extracted in a non‑accurate way but faster than in the standard mode. If raw mode doesn't support the document format, this option is ignored and the standard mode is used.

- Extract text in Accurate mode (https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
- Extract text in Raw mode (https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

The TextOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.options/textoptions/__init__/) | Initializes a new instance of the [`TextOptions`](/parser/python-net/groupdocs.parser.options/textoptions/) class. |
| [__init__](/parser/python-net/groupdocs.parser.options/textoptions/__init__/#use_raw_mode_if_possible) | Initializes a new TextOptions instance. |
| [__init__](/parser/python-net/groupdocs.parser.options/textoptions/__init__/#use_raw_mode_if_possible-use_ocr) | Initializes a new TextOptions instance with the OCR usage option. |
| [__init__](/parser/python-net/groupdocs.parser.options/textoptions/__init__/#use_raw_mode_if_possible-use_ocr-ocr_options) | Initializes a new TextOptions instance with OCR options support. |

### Properties
| Property | Description |
| :- | :- |
| [include_annotations](/parser/python-net/groupdocs.parser.options/textoptions/include_annotations/) | The value indicating whether annotations are included. |
| [ocr_options](/parser/python-net/groupdocs.parser.options/textoptions/ocr_options/) | The additional OCR options for text extraction. |
| [use_ocr](/parser/python-net/groupdocs.parser.options/textoptions/use_ocr/) | The value indicates whether the OCR Connector is used to extract text. Returns True if the OCR functionality is used; otherwise False. |
| [use_raw_mode_if_possible](/parser/python-net/groupdocs.parser.options/textoptions/use_raw_mode_if_possible/) | The value indicating whether raw mode is used. True if raw mode is used; otherwise, False. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import TextOptions

parser = Parser("sample.docx")
options = TextOptions()  # use raw mode
text = parser.get_text(options)
print(text)
```

### See Also
* module [`groupdocs.parser.options`](/parser/python-net/groupdocs.parser.options/)

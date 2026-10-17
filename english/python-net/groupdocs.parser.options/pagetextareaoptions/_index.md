---
title: PageTextAreaOptions class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Provides the options which are used for page text areas extraction."
type: docs
url: /python-net/groupdocs.parser.options/pagetextareaoptions/
is_root: false
weight: 340
---


## PageTextAreaOptions class

Provides the options which are used for page text areas extraction.

An instance of [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/) is used as a parameter in [`Parser.get_text_areas`](/parser/python-net/groupdocs.parser/parser/get_text_areas/) and [`Parser.get_text_areas`](/parser/python-net/groupdocs.parser/parser/get_text_areas/) methods. See the usage examples there.

Learn more:
- [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

The PageTextAreaOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/__init__/) | Initializes a new PageTextAreaOptions instance with the OCR usage option. |
| [__init__](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/__init__/#use_ocr) | Initializes a new instance of the [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/) class with the OCR usage option. |
| [__init__](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/__init__/#use_ocr-ocr_options) | Initializes a new instance of the PageTextAreaOptions class with the ability to set OCR options. |
| [__init__](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/__init__/#expression) | Initializes a new [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/) instance with the regular expression. |
| [__init__](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/__init__/#expression-rectangle) | Initializes a new [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/) instance with the regular expression and rectangular area, leaving other options at their default values. |
| [__init__](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/__init__/#expression-rectangle-rectangle_tolerance) | Initializes a new instance of the PageTextAreaOptions class with the regular expression, rectangular area and the size of the ignored border. |
| [__init__](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/__init__/#expression-match_case-unite_segments-ignore_formatting-rectangle) | Initializes a new PageTextAreaOptions instance. |
| [__init__](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/__init__/#expression-match_case-unite_segments-ignore_formatting-rectangle-rectangle_tolerance) | Initializes a new PageTextAreaOptions instance with the size of the ignored border. |

### Properties
| Property | Description |
| :- | :- |
| [expression](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/expression/) | The regular expression used to filter text areas. |
| [ignore_formatting](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/ignore_formatting/) | The value indicating whether text formatting is ignored. True if text formatting is ignored; otherwise, False. |
| [match_case](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/match_case/) | The value indicating whether a text case isn't ignored. |
| [ocr_options](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/ocr_options/) | The additional OCR options for extracting text areas. |
| [unite_segments](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/unite_segments/) | The value indicating whether segments are united. |
| [use_ocr](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/use_ocr/) | The flag indicating whether OCR functionality is used to extract text areas. |
| [rectangle](/parser/python-net/groupdocs.parser.options/pageareaoptions/rectangle/) | The rectangular area that contains page areas. (inherited from [`PageAreaOptions`](/parser/python-net/groupdocs.parser.options/pageareaoptions/)) |
| [rectangle_tolerance](/parser/python-net/groupdocs.parser.options/pageareaoptions/rectangle_tolerance/) | The size of the border that is ignored when captured by the rectangular area, measured as a fraction of a text item height. (inherited from [`PageAreaOptions`](/parser/python-net/groupdocs.parser.options/pageareaoptions/)) |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import PageTextAreaOptions

options = PageTextAreaOptions()
text_areas = Parser("sample.docx").get_text_areas(options)
```

### See Also
* module [`groupdocs.parser.options`](/parser/python-net/groupdocs.parser.options/)

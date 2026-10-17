---
title: HighlightOptions class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Provides the options which are used to extract a highlight (a block of text around found text in search scenarios)."
type: docs
url: /python-net/groupdocs.parser.options/highlightoptions/
is_root: false
weight: 180
---


## HighlightOptions class

Provides the options which are used to extract a highlight (a block of text around found text in search scenarios).

An instance of [`HighlightOptions`](/parser/python-net/groupdocs.parser.options/highlightoptions/) is used as a parameter in `Parser.get_highlight(int, bool, HighlightOptions)` method. See the usage examples there.

Learn more:
- Extract highlights (https://docs.groupdocs.com/display/parsernet/Extract+highlights)

The HighlightOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.options/highlightoptions/__init__/) | Initializes a new instance of the [`HighlightOptions`](/parser/python-net/groupdocs.parser.options/highlightoptions/) class which is used to extract a fixed-length highlight. |
| [__init__](/parser/python-net/groupdocs.parser.options/highlightoptions/__init__/#max_length) | Initializes a new HighlightOptions instance used to extract a fixed-length highlight. |
| [__init__](/parser/python-net/groupdocs.parser.options/highlightoptions/__init__/#max_length-is_line_limited) | Initializes a new instance of the [`HighlightOptions`](/parser/python-net/groupdocs.parser.options/highlightoptions/) class which is used to extract a line‑limited highlight. |
| [__init__](/parser/python-net/groupdocs.parser.options/highlightoptions/__init__/#max_length-word_count) | Initializes a new HighlightOptions instance used to extract a highlight with a fixed word count. |
| [__init__](/parser/python-net/groupdocs.parser.options/highlightoptions/__init__/#max_length-word_count-is_line_limited) | Initializes a new HighlightOptions instance. |

### Properties
| Property | Description |
| :- | :- |
| [is_line_limited](/parser/python-net/groupdocs.parser.options/highlightoptions/is_line_limited/) | The value indicating whether highlight extraction is limited by the start (or the end) of a text line. |
| [max_length](/parser/python-net/groupdocs.parser.options/highlightoptions/max_length/) | The maximum text length. |
| [word_count](/parser/python-net/groupdocs.parser.options/highlightoptions/word_count/) | The maximum word count. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import HighlightOptions

parser = Parser("sample.docx")
options = HighlightOptions(20)
highlight = parser.get_highlight(1, True, options)
print(highlight.text)
```

### See Also
* module [`groupdocs.parser.options`](/parser/python-net/groupdocs.parser.options/)

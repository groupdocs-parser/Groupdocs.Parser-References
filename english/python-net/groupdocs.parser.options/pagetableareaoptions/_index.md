---
title: PageTableAreaOptions class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Provides options used for page table area extraction."
type: docs
url: /python-net/groupdocs.parser.options/pagetableareaoptions/
is_root: false
weight: 330
---


## PageTableAreaOptions class

Provides options used for page table area extraction.

An instance of [`PageTableAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetableareaoptions/) class is used as a parameter in [`Parser.get_tables`](/parser/python-net/groupdocs.parser/parser/get_tables/) and [`Parser.get_tables`](/parser/python-net/groupdocs.parser/parser/get_tables/) methods.

The PageTableAreaOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.options/pagetableareaoptions/__init__/#table_layout) | Initializes a new PageAreaOptions instance. |

### Properties
| Property | Description |
| :- | :- |
| [table_layout](/parser/python-net/groupdocs.parser.options/pagetableareaoptions/table_layout/) | The table layout which defines the table on a page. |
| [rectangle](/parser/python-net/groupdocs.parser.options/pageareaoptions/rectangle/) | The rectangular area that contains page areas. (inherited from [`PageAreaOptions`](/parser/python-net/groupdocs.parser.options/pageareaoptions/)) |
| [rectangle_tolerance](/parser/python-net/groupdocs.parser.options/pageareaoptions/rectangle_tolerance/) | The size of the border that is ignored when captured by the rectangular area, measured as a fraction of a text item height. (inherited from [`PageAreaOptions`](/parser/python-net/groupdocs.parser.options/pageareaoptions/)) |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import PageTableAreaOptions
from groupdocs.parser.templates import TemplateTableLayout

parser = Parser("sample.docx")
options = PageTableAreaOptions(TemplateTableLayout([50.0, 95.0, 275.0], [325.0, 340.0, 365.0]))
tables = parser.get_tables(options)
```

### See Also
* module [`groupdocs.parser.options`](/parser/python-net/groupdocs.parser.options/)

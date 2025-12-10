---
title: PageTableAreaOptions class
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.options/pagetableareaoptions/
is_root: false
weight: 290
---

## PageTableAreaOptions class

Provides the options which are used for page table areas extraction.



**Inheritance:** [`PageTableAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetableareaoptions) → 
[`PageAreaOptions`](/parser/python-net/groupdocs.parser.options/pageareaoptions)



The PageTableAreaOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.options/pagetableareaoptions/__init__/#groupdocs.parser.templates.TemplateTableLayout) | Initializes a new instance of the [`PageAreaOptions`](/parser/python-net/groupdocs.parser.options/pageareaoptions) class. |


### Properties
| Property | Description |
| :- | :- |
| [rectangle](/parser/python-net/groupdocs.parser.options/pagetableareaoptions/rectangle) | Gets the rectangular area that contains page areas. |
| [rectangle_tolerance](/parser/python-net/groupdocs.parser.options/pagetableareaoptions/rectangle_tolerance) | Gets the size of the border that is ignored when captured by the rectangular area. It's measured by the fraction of a text item height. |
| [table_layout](/parser/python-net/groupdocs.parser.options/pagetableareaoptions/table_layout) | Gets the table layout which defines the table on a page. |



### Remarks 


An instance of [`PageTableAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetableareaoptions) class is used as parameter 
in [`Parser.get_tables`](/parser/python-net/groupdocs.parser/parser/get_tables) and [`Parser.get_tables`](/parser/python-net/groupdocs.parser/parser/get_tables) methods.
See the usage examples there.

### See Also
* module [`groupdocs.parser.options`](..)
* class [`PageAreaOptions`](/parser/python-net/groupdocs.parser.options/pageareaoptions)
* class [`PageTableAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetableareaoptions)

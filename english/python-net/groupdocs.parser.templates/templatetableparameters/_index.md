---
title: TemplateTableParameters class
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.templates/templatetableparameters/
is_root: false
weight: 140
---

## TemplateTableParameters class

Provides parameters for the table detection algorithms.



The TemplateTableParameters type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.templates/templatetableparameters/__init__/#groupdocs.parser.data.Rectangle-list) | Constructs a new instance of TemplateTableParameters |
| [__init__](/parser/python-net/groupdocs.parser.templates/templatetableparameters/__init__/#groupdocs.parser.data.Rectangle-list-System.Nullable`1[[System.Boolean]]-System.Nullable`1[[System.Int32]]-System.Nullable`1[[System.Int32]]-System.Nullable`1[[System.Int32]]) | Constructs a new instance of TemplateTableParameters |


### Properties
| Property | Description |
| :- | :- |
| [rectangle](/parser/python-net/groupdocs.parser.templates/templatetableparameters/rectangle) | Gets the rectangular area that contains the table. |
| [has_merged_cells](/parser/python-net/groupdocs.parser.templates/templatetableparameters/has_merged_cells) | Gets the value that indicates whether the table has merged cells. |
| [min_row_count](/parser/python-net/groupdocs.parser.templates/templatetableparameters/min_row_count) | Gets the minimum number of the table rows. |
| [min_column_count](/parser/python-net/groupdocs.parser.templates/templatetableparameters/min_column_count) | Gets the minimum number of the table columns. |
| [min_vertical_space](/parser/python-net/groupdocs.parser.templates/templatetableparameters/min_vertical_space) | Gets the minumum space between the table columns. |
| [vertical_separators](/parser/python-net/groupdocs.parser.templates/templatetableparameters/vertical_separators) | Gets the table columns separators. |



### Remarks 


There are two algorithms to detect a table:

|
|
 |
 |



In some cases when algorithms can't detect a table or do it in non-accurate way
[`TemplateTableLayout`](/parser/python-net/groupdocs.parser.templates/templatetablelayout) class is used.

### See Also
* module [`groupdocs.parser.templates`](..)
* class [`TemplateTableLayout`](/parser/python-net/groupdocs.parser.templates/templatetablelayout)

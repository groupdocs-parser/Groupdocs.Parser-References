---
title: PageRenderInfo class
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.options/pagerenderinfo/
is_root: false
weight: 280
---

## PageRenderInfo class

Represents the information of how a page is rendered.



The PageRenderInfo type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.options/pagerenderinfo/__init__/#int-int-int) | Initializes a new instance of the [`PageRenderInfo`](/parser/python-net/groupdocs.parser.options/pagerenderinfo) class. |


### Properties
| Property | Description |
| :- | :- |
| [page_number](/parser/python-net/groupdocs.parser.options/pagerenderinfo/page_number) | Gets the page number. |
| [row_count](/parser/python-net/groupdocs.parser.options/pagerenderinfo/row_count) | Get the total number of tiles rows. |
| [column_count](/parser/python-net/groupdocs.parser.options/pagerenderinfo/column_count) | Get the total number of tiles columns. |


### Methods
| Method | Description |
| :- | :- |
| [get_column](/parser/python-net/groupdocs.parser.options/pagerenderinfo/get_column/#int) | Returns the index of column where the tile with `tile_index` is placed. |
| [get_row](/parser/python-net/groupdocs.parser.options/pagerenderinfo/get_row/#int) | Returns the index of row where the tile with `tile_index` is placed. |



### Remarks 


Some documents (spreadsheets, for example) are not possible to render a page 
as a single image. For those documents a page is rendered as a set of tiles. 
These tiles are placed in the rectangular table.


[`PageRenderInfo.row_count`](/parser/python-net/groupdocs.parser.options/pagerenderinfo#row_count) and [`PageRenderInfo.column_count`](/parser/python-net/groupdocs.parser.options/pagerenderinfo#column_count) 
represent the total number of rows and columns of this table. If document page is rendered
to the single image these properties are equal to 1.

### See Also
* module [`groupdocs.parser.options`](..)
* class [`PageRenderInfo`](/parser/python-net/groupdocs.parser.options/pagerenderinfo)

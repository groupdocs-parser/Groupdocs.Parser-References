---
title: PageRenderInfo class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Represents the information of how a page is rendered."
type: docs
url: /python-net/groupdocs.parser.options/pagerenderinfo/
is_root: false
weight: 320
---


## PageRenderInfo class

Represents the information of how a page is rendered.

Some documents (spreadsheets, for example) are not possible to render a page as a single image. For those documents a page is rendered as a set of tiles. These tiles are placed in the rectangular table.

[`PageRenderInfo.row_count`](/parser/python-net/groupdocs.parser.options/pagerenderinfo/row_count/) and [`PageRenderInfo.column_count`](/parser/python-net/groupdocs.parser.options/pagerenderinfo/column_count/) represent the total number of rows and columns of this table. If document page is rendered to the single image these properties are equal to 1.

The PageRenderInfo type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.options/pagerenderinfo/__init__/#page_number-row_count-column_count) | Initializes a new PageRenderInfo instance. |

### Methods
| Method | Description |
| :- | :- |
| [get_column](/parser/python-net/groupdocs.parser.options/pagerenderinfo/get_column/#tile_index) | Returns the column index for the specified tile. |
| [get_column_int32](/parser/python-net/groupdocs.parser.options/pagerenderinfo/get_column_int32/) |  |
| [get_row](/parser/python-net/groupdocs.parser.options/pagerenderinfo/get_row/#tile_index) | Returns the index of the row where the tile with the specified tile index is placed. |
| [get_row_int32](/parser/python-net/groupdocs.parser.options/pagerenderinfo/get_row_int32/) |  |

### Properties
| Property | Description |
| :- | :- |
| [column_count](/parser/python-net/groupdocs.parser.options/pagerenderinfo/column_count/) | The total number of tile columns. |
| [page_number](/parser/python-net/groupdocs.parser.options/pagerenderinfo/page_number/) | The page number. |
| [row_count](/parser/python-net/groupdocs.parser.options/pagerenderinfo/row_count/) | The total number of tile rows. |

### See Also
* module [`groupdocs.parser.options`](/parser/python-net/groupdocs.parser.options/)

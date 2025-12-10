---
title: PreviewOptions class
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.options/previewoptions/
is_root: false
weight: 330
---

## PreviewOptions class

Provides options to sets requirements and stream delegates for preview generation.



The PreviewOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.options/previewoptions/__init__/#groupdocs.parser.options.ICreatePageStream) | Initializes a new instance of the [`PreviewOptions`](/parser/python-net/groupdocs.parser.options/previewoptions) class causing the output stream to be closed. |
| [__init__](/parser/python-net/groupdocs.parser.options/previewoptions/__init__/#groupdocs.parser.options.ICreatePageStream-groupdocs.parser.options.IReleasePageStream) | Initializes a new instance of [`PreviewOptions`](/parser/python-net/groupdocs.parser.options/previewoptions) class causing the output stream to be returned to the client for further use. |


### Properties
| Property | Description |
| :- | :- |
| [width](/parser/python-net/groupdocs.parser.options/previewoptions/width) | Gets or sets the page preview width. |
| [height](/parser/python-net/groupdocs.parser.options/previewoptions/height) | Gets or sets the page preview height. |
| [page_numbers](/parser/python-net/groupdocs.parser.options/previewoptions/page_numbers) | Gets or sets an array of page numbers to generate previews. |
| [preview_format](/parser/python-net/groupdocs.parser.options/previewoptions/preview_format) | Gets or sets the preview image format. |
| [create_page_stream](/parser/python-net/groupdocs.parser.options/previewoptions/create_page_stream) | Gets or sets an instance of the page stream creation delegate. |
| [release_page_stream](/parser/python-net/groupdocs.parser.options/previewoptions/release_page_stream) | Gets or sets an instance of the page preview completion delegate. |
| [dpi](/parser/python-net/groupdocs.parser.options/previewoptions/dpi) | Gets or sets a dpi. |
| [preview_page_render](/parser/python-net/groupdocs.parser.options/previewoptions/preview_page_render) | Gets or sets an instance of the page preview render info delegate. |



### See Also
* module [`groupdocs.parser.options`](..)
* class [`PreviewOptions`](/parser/python-net/groupdocs.parser.options/previewoptions)

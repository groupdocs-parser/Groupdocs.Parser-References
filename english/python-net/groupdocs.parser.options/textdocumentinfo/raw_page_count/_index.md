---
title: raw_page_count property
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.options/textdocumentinfo/raw_page_count/
is_root: false
weight: 70
---

## raw_page_count property


Gets the total number of document raw pages.

### Remarks 


Use [`DocumentInfo.raw_page_count`](/parser/python-net/groupdocs.parser.options/documentinfo#raw_page_count) property instead of [`DocumentInfo.page_count`](/parser/python-net/groupdocs.parser.options/documentinfo#page_count) property for raw text extraction.
Some documents have different page numbers in accurate and raw text extraction modes.
[`DocumentInfo.page_count`](/parser/python-net/groupdocs.parser.options/documentinfo#page_count) property may perform extra calculations which impacts on text extraction speed in raw mode.

### See Also
* module [`groupdocs.parser.options`](../../)
* class [`TextDocumentInfo`](/parser/python-net/groupdocs.parser.options/textdocumentinfo)

---
title: raw_page_count property
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.options/idocumentinfo/raw_page_count/
is_root: false
weight: 60
---

## raw_page_count property


Gets the total number of document raw pages.

### Remarks 


Use [`IDocumentInfo.raw_page_count`](/parser/python-net/groupdocs.parser.options/idocumentinfo#raw_page_count) property instead of [`IDocumentInfo.page_count`](/parser/python-net/groupdocs.parser.options/idocumentinfo#page_count) property for raw text extraction.
Some documents have different page numbers in accurate and raw text extraction modes.
[`IDocumentInfo.page_count`](/parser/python-net/groupdocs.parser.options/idocumentinfo#page_count) property may perform extra calculations which impacts on text extraction speed in raw mode.
### Definition:
```python
@property
def raw_page_count(self):
    ...
```

### See Also
* module [`groupdocs.parser.options`](../../)
* class [`IDocumentInfo`](/parser/python-net/groupdocs.parser.options/idocumentinfo)

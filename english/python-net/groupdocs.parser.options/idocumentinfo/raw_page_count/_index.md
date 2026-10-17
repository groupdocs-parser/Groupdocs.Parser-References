---
title: raw_page_count property
second_title: GroupDocs.Parser for Python via .NET API References
description: "The total number of document raw pages."
type: docs
url: /python-net/groupdocs.parser.options/idocumentinfo/raw_page_count/
is_root: false
weight: 2040
---


## raw_page_count property

The total number of document raw pages.

Use [`IDocumentInfo.raw_page_count`](/parser/python-net/groupdocs.parser.options/idocumentinfo/raw_page_count/) property instead of [`IDocumentInfo.page_count`](/parser/python-net/groupdocs.parser.options/idocumentinfo/page_count/) for raw text extraction. Some documents have different page numbers in accurate and raw text extraction modes. The [`IDocumentInfo.page_count`](/parser/python-net/groupdocs.parser.options/idocumentinfo/page_count/) property may perform extra calculations which impacts text extraction speed in raw mode.

### Definition:
```python
@property
def raw_page_count(self):
    ...
```

### See Also
* class [`IDocumentInfo`](/parser/python-net/groupdocs.parser.options/idocumentinfo/)

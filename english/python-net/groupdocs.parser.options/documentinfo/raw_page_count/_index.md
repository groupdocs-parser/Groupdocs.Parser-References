---
title: raw_page_count property
second_title: GroupDocs.Parser for Python via .NET API References
description: "The total number of raw pages in the document."
type: docs
url: /python-net/groupdocs.parser.options/documentinfo/raw_page_count/
is_root: false
weight: 2040
---


## raw_page_count property

The total number of raw pages in the document.

Use [`DocumentInfo.raw_page_count`](/parser/python-net/groupdocs.parser.options/documentinfo/raw_page_count/) instead of [`DocumentInfo.page_count`](/parser/python-net/groupdocs.parser.options/documentinfo/page_count/) for raw text extraction. Some documents have different page numbers in accurate and raw text extraction modes. The [`DocumentInfo.page_count`](/parser/python-net/groupdocs.parser.options/documentinfo/page_count/) property may perform extra calculations which impacts text extraction speed in raw mode.

### Definition:
```python
@property
def raw_page_count(self):
    ...
```

### See Also
* class [`DocumentInfo`](/parser/python-net/groupdocs.parser.options/documentinfo/)

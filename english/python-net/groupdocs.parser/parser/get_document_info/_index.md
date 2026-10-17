---
title: get_document_info method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Returns the general information about the document."
type: docs
url: /python-net/groupdocs.parser/parser/get_document_info/
is_root: false
weight: 1130
---


## get_document_info

Returns the general information about the document.

Learn more:
- https://docs.groupdocs.com/display/parsernet/Get+document+info
- https://docs.groupdocs.com/display/parsernet/Detect+encoding

```python
def get_document_info(self):
    ...
```

**Returns:** IDocumentInfo

### Example

```python
from groupdocs.parser import Parser

with Parser("./sample.docx") as parser:
    doc_info = parser.get_document_info()
    print(f"File type: {doc_info.file_type.file_format}")
    print(f"Page count: {doc_info.page_count}")
    print(f"Size: {doc_info.size} bytes")
```

### See Also
* class [`Parser`](/parser/python-net/groupdocs.parser/parser/)

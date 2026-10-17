---
title: get_metadata method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Extracts metadata from the document."
type: docs
url: /python-net/groupdocs.parser/parser/get_metadata/
is_root: false
weight: 1300
---


## get_metadata

Extracts metadata from the document.

Learn more:
- Extract metadata from documents (https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+documents)
- Extract metadata from Microsoft Office Word documents (https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+Word+documents)
- Extract metadata from Microsoft Office Excel spreadsheets (https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+Excel+spreadsheets)
- Extract metadata from Microsoft Office PowerPoint presentations (https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+PowerPoint+presentations)
- Extract metadata from PDF documents (https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+PDF+documents)
- Extract metadata from Emails (https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Emails)

```python
def get_metadata(self):
    ...
```

**Returns:** Iterable[MetadataItem] or None: A collection of metadata items; None if metadata extraction isn't supported.

### Example

```python
from groupdocs.parser import Parser

with Parser("./sample.pdf") as parser:
    metadata_items = parser.get_metadata()
    if metadata_items is None:
        print("Metadata extraction is not supported for this format.")
    else:
        for item in metadata_items:
            print(f"{item.name}: {item.value}")
```

### See Also
* class [`Parser`](/parser/python-net/groupdocs.parser/parser/)

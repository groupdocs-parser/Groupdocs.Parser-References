---
title: get_supported_file_types method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Retrieves supported file types."
type: docs
url: /python-net/groupdocs.parser.options/filetype/get_supported_file_types/
is_root: false
weight: 1060
---


## get_supported_file_types

Retrieves supported file types.

```python
def get_supported_file_types(cls):
    ...
```

**Returns:** Iterable[FileType]: Sequence of supported file types.

### Example

```python
from groupdocs.parser.options import FileType

supported_file_types = FileType.get_supported_file_types()
for ft in supported_file_types:
    print(ft)
```

### See Also
* class [`FileType`](/parser/python-net/groupdocs.parser.options/filetype/)

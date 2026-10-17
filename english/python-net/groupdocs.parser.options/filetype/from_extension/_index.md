---
title: from_extension method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Maps file extension to file type."
type: docs
url: /python-net/groupdocs.parser.options/filetype/from_extension/
is_root: false
weight: 1040
---


## from_extension {#extension}

Maps file extension to file type.

```python
def from_extension(cls, extension):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| extension | `str` | File extension (including the period "."). |

**Returns:** FileType: When file type is supported returns it, otherwise returns default `FileType.unknown` file type.

| Raises | Description |
| :- | :- |
| `ValueError` | When `extension` is null or empty string. |

### See Also
* class [`FileType`](/parser/python-net/groupdocs.parser.options/filetype/)

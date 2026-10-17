---
title: try_parse method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Converts the string representation of a size to its class equivalent."
type: docs
url: /python-net/groupdocs.parser.data/size/try_parse/
is_root: false
weight: 1030
---


## try_parse {#s-size}

Converts the string representation of a size to its class equivalent.

```python
def try_parse(cls, s, size):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| s | `str` | A string containing a size to convert. |
| size | `Size` | When the method returns, contains the instance of `Size` that is equivalent to the value specified in `s` if the conversion succeeded; otherwise, `None`. |

**Returns:** bool: `True` if `s` is converted successfully; otherwise, `False`.

### See Also
* class [`Size`](/parser/python-net/groupdocs.parser.data/size/)

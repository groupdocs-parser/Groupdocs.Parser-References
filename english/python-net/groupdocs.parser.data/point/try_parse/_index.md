---
title: try_parse method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Converts the string representation of a point to its class equivalent."
type: docs
url: /python-net/groupdocs.parser.data/point/try_parse/
is_root: false
weight: 1070
---


## try_parse {#s-point}

Converts the string representation of a point to its class equivalent.

```python
def try_parse(cls, s, point):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| s | `str` | A string containing a point to convert. |
| point | `Point` | When the method returns, contains the `Point` instance equivalent to the value specified in `s` if conversion succeeded; otherwise, `None`. |

**Returns:** bool: `True` if `s` was converted successfully; otherwise, `False`.

### See Also
* class [`Point`](/parser/python-net/groupdocs.parser.data/point/)

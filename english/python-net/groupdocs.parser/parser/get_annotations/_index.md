---
title: get_annotations method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Extracts annotations from the document."
type: docs
url: /python-net/groupdocs.parser/parser/get_annotations/
is_root: false
weight: 1040
---


## get_annotations

Extracts annotations from the document.

```python
def get_annotations(self):
    ...
```

**Returns:** A collection of annotation items; None if annotation extraction isn't supported.

## get_annotations {#page_index}

Extracts annotations from the document page.

```python
def get_annotations(self, page_index):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| page_index | `int` | The zero-based page index. |

**Returns:** A collection of annotation items; None if annotation extraction isn't supported.

### Aliases

These names call `get_annotations` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_annotations_int32` | `get_annotations_int32(page_index)` |

### See Also
* class [`Parser`](/parser/python-net/groupdocs.parser/parser/)

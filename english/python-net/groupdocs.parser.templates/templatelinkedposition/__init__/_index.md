---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new instance of the TemplateLinkedPosition class."
type: docs
url: /python-net/groupdocs.parser.templates/templatelinkedposition/__init__/
is_root: false
weight: 10
---


## __init__ {#linked_field_name-search_area-edges}

Initializes a new instance of the [`TemplateLinkedPosition`](/parser/python-net/groupdocs.parser.templates/templatelinkedposition/) class.

```python
def __init__(self, linked_field_name, search_area, edges):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| linked_field_name | `str` | The name of the linked field. |
| search_area | `Size` | The size of the area where a field is searched. |
| edges | `TemplateLinkedPositionEdges` | The edges of the linked field where a field is searched. |

## __init__ {#linked_field_name-search_area-edges-auto_scale}

Initializes a new instance of TemplateLinkedPosition with an upper‑case linked field name.

```python
def __init__(self, linked_field_name, search_area, edges, auto_scale):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| linked_field_name | `str` | The name of the linked field. |
| search_area | `Size` | The size of the area where a field is searched. |
| edges | `TemplateLinkedPositionEdges` | The edges of the linked field where a field is searched. |
| auto_scale | `bool` | The value that indicates whether `search_area` is scaled by the linked field size. |

## __init__ {#linked_field_name-search_area-edges-auto_scale-use_upper_case_name}

Initializes a new TemplateLinkedPosition instance.

```python
def __init__(self, linked_field_name, search_area, edges, auto_scale, use_upper_case_name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| linked_field_name | `str` | The name of the linked field. |
| search_area | `Size` | The size of the area where a field is searched. |
| edges | `TemplateLinkedPositionEdges` | The edges of the linked field where a field is searched. |
| auto_scale | `bool` | The value that indicates whether `search_area` is scaled by the linked field size. |
| use_upper_case_name | `bool` | The value that indicates whether a `name` is converted to UPPER CASE. |

### See Also
* class [`TemplateLinkedPosition`](/parser/python-net/groupdocs.parser.templates/templatelinkedposition/)

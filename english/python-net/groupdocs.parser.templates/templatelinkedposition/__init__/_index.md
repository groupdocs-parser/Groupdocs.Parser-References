---
title: TemplateLinkedPosition constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.templates/templatelinkedposition/__init__/
is_root: false
weight: 10
---

## __init__ {#System.String-groupdocs.parser.data.Size-groupdocs.parser.templates.TemplateLinkedPositionEdges}

Initializes a new instance of the [`TemplateLinkedPosition`](/parser/python-net/groupdocs.parser.templates/templatelinkedposition) class.



```python
def __init__(self, linked_field_name, search_area, edges):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| linked_field_name | System.String | The name of the linked field. |
| search_area | groupdocs.parser.data.Size | The size of the area where a field is searched. |
| edges | groupdocs.parser.templates.TemplateLinkedPositionEdges | The edges of the linked field where a field is searched. |


## __init__ {#System.String-groupdocs.parser.data.Size-groupdocs.parser.templates.TemplateLinkedPositionEdges-bool}

Initializes a new instance of the [`TemplateLinkedPosition`](/parser/python-net/groupdocs.parser.templates/templatelinkedposition) class with UPPER CASE linked field name.



```python
def __init__(self, linked_field_name, search_area, edges, auto_scale):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| linked_field_name | System.String | The name of the linked field. |
| search_area | groupdocs.parser.data.Size | The size of the area where a field is searched. |
| edges | groupdocs.parser.templates.TemplateLinkedPositionEdges | The edges of the linked field where a field is searched. |
| auto_scale | bool | The value that indicates whether `search_area` is scaled by the linked field size. |


## __init__ {#System.String-groupdocs.parser.data.Size-groupdocs.parser.templates.TemplateLinkedPositionEdges-bool-bool}

Initializes a new instance of the [`TemplateLinkedPosition`](/parser/python-net/groupdocs.parser.templates/templatelinkedposition) class.



```python
def __init__(self, linked_field_name, search_area, edges, auto_scale, use_upper_case_name):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| linked_field_name | System.String | The name of the linked field. |
| search_area | groupdocs.parser.data.Size | The size of the area where a field is searched. |
| edges | groupdocs.parser.templates.TemplateLinkedPositionEdges | The edges of the linked field where a field is searched. |
| auto_scale | bool | The value that indicates whether `search_area` is scaled by the linked field size. |
| use_upper_case_name | bool | The value that indicates whether a `name` is converted to UPPER CASE. |



### See Also
* module [`groupdocs.parser.templates`](../../)
* class [`TemplateLinkedPosition`](/parser/python-net/groupdocs.parser.templates/templatelinkedposition)

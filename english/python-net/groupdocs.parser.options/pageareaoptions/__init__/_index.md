---
title: PageAreaOptions constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.options/pageareaoptions/__init__/
is_root: false
weight: 10
---

## __init__ {#}

Initializes a new instance of the [`PageAreaOptions`](/parser/python-net/groupdocs.parser.options/pageareaoptions) class.



```python
def __init__(self):
    ...
```




## __init__ {#groupdocs.parser.data.Rectangle}

Initializes a new instance of the [`PageAreaOptions`](/parser/python-net/groupdocs.parser.options/pageareaoptions) class.



```python
def __init__(self, rectangle):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| rectangle | groupdocs.parser.data.Rectangle | The rectangular area that contains page areas. |


## __init__ {#groupdocs.parser.data.Rectangle-float}

Initializes a new instance of the [`PageAreaOptions`](/parser/python-net/groupdocs.parser.options/pageareaoptions) class with the size of the ignored border.



```python
def __init__(self, rectangle, rectangle_tolerance):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| rectangle | groupdocs.parser.data.Rectangle | The rectangular area that contains page areas. |
| rectangle_tolerance | float | The size of the border that is ignored when captured by the rectangular area. It's measured by the fraction of a text item height. |



### See Also
* module [`groupdocs.parser.options`](../../)
* class [`PageAreaOptions`](/parser/python-net/groupdocs.parser.options/pageareaoptions)

---
title: PageTextAreaOptions constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.options/pagetextareaoptions/__init__/
is_root: false
weight: 10
---

## __init__ {#}

Initializes a new instance of the [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions) class with the OCR usage option.



```python
def __init__(self):
    ...
```




## __init__ {#bool}

Initializes a new instance of the [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions) class with the OCR usage option.



```python
def __init__(self, use_ocr):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| use_ocr | bool | The value that indicates whether OCR functionality is used to extract text areas. |


## __init__ {#System.String}

Initializes a new instance of the [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions) class with the regular expression. 
Other options are set by default (see remarks for details).



```python
def __init__(self, expression):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| expression | System.String | The regular expression. |


## __init__ {#bool-groupdocs.parser.options.OcrOptions}

Initializes a new instance of the [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions) class with the ability to set OCR options.



```python
def __init__(self, use_ocr, ocr_options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| use_ocr | bool | The value that indicates whether OCR functionality is used to extract text areas. |
| ocr_options | groupdocs.parser.options.OcrOptions | The additional options for OCR functionality. |


## __init__ {#System.String-groupdocs.parser.data.Rectangle}

Initializes a new instance of the [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions) class
with the regular expression and rectangular area. 
Other options are set by default (see remarks for details).



```python
def __init__(self, expression, rectangle):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| expression | System.String | The regular expression. |
| rectangle | groupdocs.parser.data.Rectangle | The rectangular area that contains page areas. |


## __init__ {#System.String-groupdocs.parser.data.Rectangle-float}

Initializes a new instance of the [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions) class
with the regular expression, rectangular area and the size of the ignored border. 
Other options are set by default (see remarks for details).



```python
def __init__(self, expression, rectangle, rectangle_tolerance):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| expression | System.String | The regular expression. |
| rectangle | groupdocs.parser.data.Rectangle | The rectangular area that contains page areas. |
| rectangle_tolerance | float | The size of the border that is ignored when captured by the rectangular area. It's measured by the fraction of a text item height. |


## __init__ {#System.String-bool-bool-bool-groupdocs.parser.data.Rectangle}

Initializes a new instance of the [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions) class.



```python
def __init__(self, expression, match_case, unite_segments, ignore_formatting, rectangle):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| expression | System.String | The regular expression. |
| match_case | bool | The value that indicates whether a text case isn't ignored. |
| unite_segments | bool | The value that indicates whether segments are united. |
| ignore_formatting | bool | The value that indicates whether text formatting is ignored. |
| rectangle | groupdocs.parser.data.Rectangle | The rectangular area that contains page areas. |


## __init__ {#System.String-bool-bool-bool-groupdocs.parser.data.Rectangle-float}

Initializes a new instance of the [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions) class
with the size of the ignored border.



```python
def __init__(self, expression, match_case, unite_segments, ignore_formatting, rectangle, rectangle_tolerance):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| expression | System.String | The regular expression. |
| match_case | bool | The value that indicates whether a text case isn't ignored. |
| unite_segments | bool | The value that indicates whether segments are united. |
| ignore_formatting | bool | The value that indicates whether text formatting is ignored. |
| rectangle | groupdocs.parser.data.Rectangle | The rectangular area that contains page areas. |
| rectangle_tolerance | float | The size of the border that is ignored when captured by the rectangular area. It's measured by the fraction of a text item height. |



### See Also
* module [`groupdocs.parser.options`](../../)
* class [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions)

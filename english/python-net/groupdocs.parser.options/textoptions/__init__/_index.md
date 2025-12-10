---
title: TextOptions constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.options/textoptions/__init__/
is_root: false
weight: 10
---

## __init__ {#}

Initializes a new instance of the [`TextOptions`](/parser/python-net/groupdocs.parser.options/textoptions) class.



```python
def __init__(self):
    ...
```




## __init__ {#bool}

Initializes a new instance of the [`TextOptions`](/parser/python-net/groupdocs.parser.options/textoptions) class.



```python
def __init__(self, use_raw_mode_if_possible):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| use_raw_mode_if_possible | bool | The value that indicates whether the raw mode is used. |


## __init__ {#bool-bool}

Initializes a new instance of the [`TextOptions`](/parser/python-net/groupdocs.parser.options/textoptions) class with the OCR usage option.



```python
def __init__(self, use_raw_mode_if_possible, use_ocr):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| use_raw_mode_if_possible | bool | The value that indicates whether the raw mode is used. |
| use_ocr | bool | The value that indicates whether the OCR functionality is used to extract a text. |


## __init__ {#bool-bool-groupdocs.parser.options.OcrOptions}

Initializes a new instance of the [`TextOptions`](/parser/python-net/groupdocs.parser.options/textoptions) class with the ability to set OCR options.



```python
def __init__(self, use_raw_mode_if_possible, use_ocr, ocr_options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| use_raw_mode_if_possible | bool | The value that indicates whether the raw mode is used. |
| use_ocr | bool | The value that indicates whether the OCR functionality is used to extract a text. |
| ocr_options | groupdocs.parser.options.OcrOptions | The additional options for OCR functionality. |



### See Also
* module [`groupdocs.parser.options`](../../)
* class [`TextOptions`](/parser/python-net/groupdocs.parser.options/textoptions)

---
title: ParseByTemplateOptions constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.options/parsebytemplateoptions/__init__/
is_root: false
weight: 10
---

## __init__ {#}

Initializes a new instance of the [`ParseByTemplateOptions`](/parser/python-net/groupdocs.parser.options/parsebytemplateoptions) class.



```python
def __init__(self):
    ...
```




## __init__ {#int}

Initializes a new instance of the [`ParseByTemplateOptions`](/parser/python-net/groupdocs.parser.options/parsebytemplateoptions) class.



```python
def __init__(self, page_index):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| page_index | int | The page index. |


## __init__ {#int-bool}

Initializes a new instance of the [`ParseByTemplateOptions`](/parser/python-net/groupdocs.parser.options/parsebytemplateoptions) class with the OCR usage option.



```python
def __init__(self, page_index, use_ocr):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| page_index | int | The page index. |
| use_ocr | bool | The value that indicates whether the OCR functionality is used to parse by template. |


## __init__ {#int-bool-groupdocs.parser.options.OcrOptions}

Initializes a new instance of the [`ParseByTemplateOptions`](/parser/python-net/groupdocs.parser.options/parsebytemplateoptions) class with the ability to set OCR options.



```python
def __init__(self, page_index, use_ocr, ocr_options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| page_index | int | The page index. |
| use_ocr | bool | The value that indicates whether the OCR functionality is used to parse by template. |
| ocr_options | groupdocs.parser.options.OcrOptions | The additional options for OCR functionality. |



### See Also
* module [`groupdocs.parser.options`](../../)
* class [`ParseByTemplateOptions`](/parser/python-net/groupdocs.parser.options/parsebytemplateoptions)

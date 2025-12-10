---
title: OcrOptions constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.options/ocroptions/__init__/
is_root: false
weight: 10
---

## __init__ {#}

Initializes a new instance of the [`OcrOptions`](/parser/python-net/groupdocs.parser.options/ocroptions) class with rectangular area.



```python
def __init__(self):
    ...
```




## __init__ {#groupdocs.parser.options.PagePreviewOptions}

Initializes a new instance of the [`OcrOptions`](/parser/python-net/groupdocs.parser.options/ocroptions) class with rectangular area.



```python
def __init__(self, page_preview_options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| page_preview_options | groupdocs.parser.options.PagePreviewOptions | An instance of [`OcrOptions.page_preview_options`](/parser/python-net/groupdocs.parser.options/ocroptions#page_preview_options) class that sets properties for the document page preview generation. |


## __init__ {#groupdocs.parser.data.Rectangle}

Initializes a new instance of the [`OcrOptions`](/parser/python-net/groupdocs.parser.options/ocroptions) class with rectangular area.



```python
def __init__(self, rectangle):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| rectangle | groupdocs.parser.data.Rectangle | The rectangular area that constraints the page area which is used for text recognizing. |


## __init__ {#groupdocs.parser.options.OcrEventHandler}

Initializes a new instance of the [`OcrOptions`](/parser/python-net/groupdocs.parser.options/ocroptions) class with [`OcrEventHandler`](/parser/python-net/groupdocs.parser.options/ocreventhandler) object.



```python
def __init__(self, handler):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| handler | groupdocs.parser.options.OcrEventHandler | An instance of [`OcrEventHandler`](/parser/python-net/groupdocs.parser.options/ocreventhandler) to catch OCR events. |


## __init__ {#groupdocs.parser.data.Rectangle-groupdocs.parser.options.OcrEventHandler}

Initializes a new instance of the [`OcrOptions`](/parser/python-net/groupdocs.parser.options/ocroptions) class with rectangular area and [`OcrEventHandler`](/parser/python-net/groupdocs.parser.options/ocreventhandler) object.



```python
def __init__(self, rectangle, handler):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| rectangle | groupdocs.parser.data.Rectangle | The rectangular area that constraints the page area which is used for text recognizing. |
| handler | groupdocs.parser.options.OcrEventHandler | An instance of [`OcrEventHandler`](/parser/python-net/groupdocs.parser.options/ocreventhandler) to catch OCR events. |


## __init__ {#groupdocs.parser.data.Rectangle-groupdocs.parser.options.OcrEventHandler-groupdocs.parser.options.PagePreviewOptions-bool}

Initializes a new instance of the [`OcrOptions`](/parser/python-net/groupdocs.parser.options/ocroptions) class.



```python
def __init__(self, rectangle, handler, page_preview_options, use_spell_cheker):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| rectangle | groupdocs.parser.data.Rectangle | The rectangular area that constraints the page area which is used for text recognizing. |
| handler | groupdocs.parser.options.OcrEventHandler | An instance of [`OcrEventHandler`](/parser/python-net/groupdocs.parser.options/ocreventhandler) to catch OCR events. |
| page_preview_options | groupdocs.parser.options.PagePreviewOptions | An instance of [`OcrOptions.page_preview_options`](/parser/python-net/groupdocs.parser.options/ocroptions#page_preview_options) class that sets properties for the document page preview generation. |
| use_spell_cheker | bool | The value that indicates whether the spell checker is used. |



### See Also
* module [`groupdocs.parser.options`](../../)
* class [`OcrEventHandler`](/parser/python-net/groupdocs.parser.options/ocreventhandler)
* class [`OcrOptions`](/parser/python-net/groupdocs.parser.options/ocroptions)

---
title: recognize_text_areas method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.options/ocrconnectorbase/recognize_text_areas/
is_root: false
weight: 30
---

## recognize_text_areas {#io.RawIOBase-groupdocs.parser.data.Size-groupdocs.parser.options.OcrOptions}

Recognize text areas from `image_stream` stream.


### Returns 


A collection of [`PageTextArea`](/parser/python-net/groupdocs.parser.data/pagetextarea) objects; `null` if text areas recognizing isn't supported.


```python
def recognize_text_areas(self, image_stream, page_size, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| image_stream | io.RawIOBase | The image representation of the document page. |
| page_size | groupdocs.parser.data.Size | The size of the document page. |
| options | groupdocs.parser.options.OcrOptions | The OCR options. |


## recognize_text_areas {#io.RawIOBase-groupdocs.parser.data.Page-groupdocs.parser.options.OcrOptions}

Recognize text areas from `image_stream` stream.


### Returns 


A collection of [`PageTextArea`](/parser/python-net/groupdocs.parser.data/pagetextarea) objects; `null` if text areas recognizing isn't supported.


```python
def recognize_text_areas(self, image_stream, page, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| image_stream | io.RawIOBase | The image representation of the document page. |
| page | groupdocs.parser.data.Page | The the document page. |
| options | groupdocs.parser.options.OcrOptions | The OCR options. |


## recognize_text_areas {#io.RawIOBase-int-groupdocs.parser.data.Size-groupdocs.parser.options.OcrOptions}

Recognize text areas from `image_stream` stream.


### Returns 


A collection of [`PageTextArea`](/parser/python-net/groupdocs.parser.data/pagetextarea) objects; `null` if text areas recognizing isn't supported.


```python
def recognize_text_areas(self, image_stream, page_index, page_size, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| image_stream | io.RawIOBase | The image representation of the document page. |
| page_index | int | The page index of the document. |
| page_size | groupdocs.parser.data.Size | The size of the document page. |
| options | groupdocs.parser.options.OcrOptions | The OCR options. |


## recognize_text_areas {#io.RawIOBase-list-System.String-groupdocs.parser.data.Page-groupdocs.parser.options.OcrOptions}





```python
def recognize_text_areas(self, image_stream, rectangles, allowed_symbols, page, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| image_stream | io.RawIOBase |  |
| rectangles | list |  |
| allowed_symbols | System.String |  |
| page | groupdocs.parser.data.Page |  |
| options | groupdocs.parser.options.OcrOptions |  |



### See Also
* module [`groupdocs.parser.options`](../../)
* class [`OcrConnectorBase`](/parser/python-net/groupdocs.parser.options/ocrconnectorbase)
* class [`PageTextArea`](/parser/python-net/groupdocs.parser.data/pagetextarea)

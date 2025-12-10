---
title: recognize_text method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.options/ocrconnectorbase/recognize_text/
is_root: false
weight: 20
---

## recognize_text {#io.RawIOBase-groupdocs.parser.options.OcrOptions}

Recognize a text from `image_stream` stream.


### Returns 


A string that represents a recognized text; `null` if text recognizing isn't supported.


```python
def recognize_text(self, image_stream, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| image_stream | io.RawIOBase | The image representation of the document page. |
| options | groupdocs.parser.options.OcrOptions | The OCR options. |


## recognize_text {#io.RawIOBase-int-groupdocs.parser.options.OcrOptions}

Recognize a text from `image_stream` stream.


### Returns 


A string that represents a recognized text; `null` if text recognizing isn't supported.


```python
def recognize_text(self, image_stream, page_index, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| image_stream | io.RawIOBase | The image representation of the document page. |
| page_index | int | The page index of the document. |
| options | groupdocs.parser.options.OcrOptions | The OCR options. |



### See Also
* module [`groupdocs.parser.options`](../../)
* class [`OcrConnectorBase`](/parser/python-net/groupdocs.parser.options/ocrconnectorbase)

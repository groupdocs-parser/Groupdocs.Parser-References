---
title: BarcodeOptions constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.options/barcodeoptions/__init__/
is_root: false
weight: 10
---

## __init__ {#}

Initializes a new instance of the [`BarcodeOptions`](/parser/python-net/groupdocs.parser.options/barcodeoptions) class with default values.



```python
def __init__(self):
    ...
```




## __init__ {#groupdocs.parser.data.Rectangle}

Initializes a new instance of the [`BarcodeOptions`](/parser/python-net/groupdocs.parser.options/barcodeoptions) class with the rectangular area.



```python
def __init__(self, rectangle):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| rectangle | groupdocs.parser.data.Rectangle | The rectangular area that contains barcodes. |


## __init__ {#groupdocs.parser.options.QualityMode-groupdocs.parser.options.QualityMode-list}

Initializes a new instance of the [`BarcodeOptions`](/parser/python-net/groupdocs.parser.options/barcodeoptions) class with quality settings and code types.



```python
def __init__(self, image_quality, barcode_quality, code_types):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| image_quality | groupdocs.parser.options.QualityMode | The quality of a source image. |
| barcode_quality | groupdocs.parser.options.QualityMode | The quality of a source barcode. |
| code_types | list | The types of barcodes to read. |


## __init__ {#groupdocs.parser.data.Rectangle-groupdocs.parser.options.QualityMode-groupdocs.parser.options.QualityMode-System.Nullable`1[[System.Single]]-bool-list}

Constructs a new instance of BarcodeOptions



```python
def __init__(self, rectangle, image_quality, barcode_quality, dimension, allow_incorrect_barcodes, code_types):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| rectangle | groupdocs.parser.data.Rectangle |  |
| image_quality | groupdocs.parser.options.QualityMode |  |
| barcode_quality | groupdocs.parser.options.QualityMode |  |
| dimension | System.Nullable`1[[System.Single]] |  |
| allow_incorrect_barcodes | bool |  |
| code_types | list |  |



### See Also
* module [`groupdocs.parser.options`](../../)
* class [`BarcodeOptions`](/parser/python-net/groupdocs.parser.options/barcodeoptions)

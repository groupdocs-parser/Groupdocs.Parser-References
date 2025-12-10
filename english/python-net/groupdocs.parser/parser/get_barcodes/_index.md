---
title: get_barcodes method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser/parser/get_barcodes/
is_root: false
weight: 40
---

## get_barcodes {#}

Extracts barcodes from the document.


### Returns 


A collection of [`PageBarcodeArea`](/parser/python-net/groupdocs.parser.data/pagebarcodearea) objects;
`null` if barcodes extraction isn't supported.


```python
def get_barcodes(self):
    ...
```



### Example 


The following example shows how to extract barcodes from a document:


## get_barcodes {#int}

Extracts barcodes from the document page.


### Returns 


A collection of [`PageBarcodeArea`](/parser/python-net/groupdocs.parser.data/pagebarcodearea) objects;
`null` if barcodes extraction isn't supported.


```python
def get_barcodes(self, page_index):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| page_index | int | The zero-based page index. |

### Example 


The following example shows how to extract barcodes from a document page:


## get_barcodes {#groupdocs.parser.options.PageAreaOptions}

Extracts barcodes from the document using customization options 
(to set the rectangular area that contains barcodes).


### Returns 


A collection of [`PageBarcodeArea`](/parser/python-net/groupdocs.parser.data/pagebarcodearea) objects;
`null` if barcodes extraction isn't supported.


```python
def get_barcodes(self, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| options | groupdocs.parser.options.PageAreaOptions | The options for barcodes extraction. |

### Example 


The following example shows how to extract barcodes from the upper-right corner.


## get_barcodes {#groupdocs.parser.options.BarcodeOptions}

Extracts barcodes from the document using customization options.


### Returns 


A collection of [`PageBarcodeArea`](/parser/python-net/groupdocs.parser.data/pagebarcodearea) objects;
`null` if barcodes extraction isn't supported.


```python
def get_barcodes(self, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| options | groupdocs.parser.options.BarcodeOptions | The options for barcodes extraction. |

### Example 


The following example shows how to extract barcodes from the upper-right corner.


## get_barcodes {#int-groupdocs.parser.options.PageAreaOptions}

Extracts barcodes from the document page using customization options 
(to set the rectangular area that contains barcodes).


### Returns 


A collection of [`PageBarcodeArea`](/parser/python-net/groupdocs.parser.data/pagebarcodearea) objects;
`null` if barcodes extraction isn't supported.


```python
def get_barcodes(self, page_index, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| page_index | int | The zero-based page index. |
| options | groupdocs.parser.options.PageAreaOptions | The options for barcodes extraction. |


## get_barcodes {#int-groupdocs.parser.options.BarcodeOptions}

Extracts barcodes from the document page using customization options.


### Returns 


A collection of [`PageBarcodeArea`](/parser/python-net/groupdocs.parser.data/pagebarcodearea) objects;
`null` if barcodes extraction isn't supported.


```python
def get_barcodes(self, page_index, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| page_index | int | The zero-based page index. |
| options | groupdocs.parser.options.BarcodeOptions | The options for barcodes extraction. |



### See Also
* module [`groupdocs.parser`](../../)
* class [`PageBarcodeArea`](/parser/python-net/groupdocs.parser.data/pagebarcodearea)
* class [`Parser`](/parser/python-net/groupdocs.parser/parser)

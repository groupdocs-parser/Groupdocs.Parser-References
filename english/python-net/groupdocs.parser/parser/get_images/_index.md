---
title: get_images method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser/parser/get_images/
is_root: false
weight: 110
---

## get_images {#}

Extracts images from the document.


### Returns 


A collection of [`PageImageArea`](/parser/python-net/groupdocs.parser.data/pageimagearea) objects;
`null` if images extraction isn't supported.


```python
def get_images(self):
    ...
```



### Example 


The following example shows how to extract all images from the whole document:


## get_images {#groupdocs.parser.options.PageAreaOptions}

Extracts images from the document using customization options 
(to set the rectangular area that contains images).


### Returns 


A collection of [`PageImageArea`](/parser/python-net/groupdocs.parser.data/pageimagearea) objects;
`null` if images extraction isn't supported.


```python
def get_images(self, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| options | groupdocs.parser.options.PageAreaOptions | The options for images extraction. |

### Example 


The following example shows how to extract only images from the upper-left courner:


## get_images {#int}

Extracts images from the document page.


### Returns 


A collection of [`PageImageArea`](/parser/python-net/groupdocs.parser.data/pageimagearea) objects;
`null` if images extraction isn't supported.


```python
def get_images(self, page_index):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| page_index | int | The zero-based page index. |

### Example 


To extract images from a document page the following method is used:


## get_images {#int-groupdocs.parser.options.PageAreaOptions}

Extracts images from the document page using customization options 
(to set the rectangular area that contains images).


### Returns 


A collection of [`PageImageArea`](/parser/python-net/groupdocs.parser.data/pageimagearea) objects;
`null` if images extraction isn't supported.


```python
def get_images(self, page_index, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| page_index | int | The zero-based page index. |
| options | groupdocs.parser.options.PageAreaOptions | The options for images extraction. |



### See Also
* module [`groupdocs.parser`](../../)
* class [`PageImageArea`](/parser/python-net/groupdocs.parser.data/pageimagearea)
* class [`Parser`](/parser/python-net/groupdocs.parser/parser)

---
title: get_text_areas method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser/parser/get_text_areas/
is_root: false
weight: 160
---

## get_text_areas {#}

Extracts text areas from the document.


### Returns 


A collection of [`PageTextArea`](/parser/python-net/groupdocs.parser.data/pagetextarea) objects;
`null` if text areas extraction isn't supported.


```python
def get_text_areas(self):
    ...
```



### Example 


The following example shows how to extract all text areas from the whole document:


## get_text_areas {#groupdocs.parser.options.PageTextAreaOptions}

Extracts text areas from the document using customization options (regular expression, match case, etc.).


### Returns 


A collection of [`PageTextArea`](/parser/python-net/groupdocs.parser.data/pagetextarea) objects;
`null` if text areas extraction isn't supported.


```python
def get_text_areas(self, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| options | groupdocs.parser.options.PageTextAreaOptions | The options for text area extraction. |

### Example 


The following example shows how to extract only text areas with digits from the upper-left courner:


## get_text_areas {#int}

Extracts text areas from the document page.


### Returns 


A collection of [`PageTextArea`](/parser/python-net/groupdocs.parser.data/pagetextarea) objects;
`null` if text areas extraction isn't supported.


```python
def get_text_areas(self, page_index):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| page_index | int | The zero-based page index. |

### Example 


To extract text areas from a document page the following method is used:


## get_text_areas {#int-groupdocs.parser.options.PageTextAreaOptions}

Extracts text areas from the document page using customization options (regular expression, match case, etc.).


### Returns 


A collection of [`PageTextArea`](/parser/python-net/groupdocs.parser.data/pagetextarea) objects;
`null` if text areas extraction isn't supported.


```python
def get_text_areas(self, page_index, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| page_index | int | The zero-based page index. |
| options | groupdocs.parser.options.PageTextAreaOptions | The options for text area extraction. |



### See Also
* module [`groupdocs.parser`](../../)
* class [`PageTextArea`](/parser/python-net/groupdocs.parser.data/pagetextarea)
* class [`Parser`](/parser/python-net/groupdocs.parser/parser)

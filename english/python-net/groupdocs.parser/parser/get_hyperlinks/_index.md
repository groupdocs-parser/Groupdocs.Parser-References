---
title: get_hyperlinks method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser/parser/get_hyperlinks/
is_root: false
weight: 100
---

## get_hyperlinks {#}

Extracts hyperlinks from the document.


### Returns 


A collection of [`PageHyperlinkArea`](/parser/python-net/groupdocs.parser.data/pagehyperlinkarea) objects;
`null` if hyperlinks extraction isn't supported.


```python
def get_hyperlinks(self):
    ...
```



### Example 


The following example shows how to extract all hyperlinks from the whole document:


## get_hyperlinks {#int}

Extracts hyperlinks from the document page.


### Returns 


A collection of [`PageHyperlinkArea`](/parser/python-net/groupdocs.parser.data/pagehyperlinkarea) objects;
`null` if hyperlinks extraction isn't supported.


```python
def get_hyperlinks(self, page_index):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| page_index | int | The zero-based page index. |

### Example 


The following example shows how to extract hyperlinks from the document page:


## get_hyperlinks {#groupdocs.parser.options.PageAreaOptions}

Extracts hyperlinks from the document using customization options 
(to set the rectangular area that contains hyperlinks).


### Returns 


A collection of [`PageHyperlinkArea`](/parser/python-net/groupdocs.parser.data/pagehyperlinkarea) objects;
`null` if hyperlinks extraction isn't supported.


```python
def get_hyperlinks(self, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| options | groupdocs.parser.options.PageAreaOptions | The options for hyperlinks extraction. |

### Example 


The following example shows how to extract hyperlinks from the document page area:


## get_hyperlinks {#int-groupdocs.parser.options.PageAreaOptions}

Extracts hyperlinks from the document page using customization options 
(to set the rectangular area that contains hyperlinks).


### Returns 


A collection of [`PageHyperlinkArea`](/parser/python-net/groupdocs.parser.data/pagehyperlinkarea) objects;
`null` if hyperlinks extraction isn't supported.


```python
def get_hyperlinks(self, page_index, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| page_index | int | The zero-based page index. |
| options | groupdocs.parser.options.PageAreaOptions | The options for hyperlinks extraction. |

### Example 


The following example shows how to extract hyperlinks from the document page area using customization options:



### See Also
* module [`groupdocs.parser`](../../)
* class [`PageHyperlinkArea`](/parser/python-net/groupdocs.parser.data/pagehyperlinkarea)
* class [`Parser`](/parser/python-net/groupdocs.parser/parser)

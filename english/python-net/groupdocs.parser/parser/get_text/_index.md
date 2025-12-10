---
title: get_text method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser/parser/get_text/
is_root: false
weight: 150
---

## get_text {#}

Extracts a text from the document.


### Returns 


An instance of TextReader class with the extracted text;
`null` if text extraction isn't supported.


```python
def get_text(self):
    ...
```



### Example 


The following example shows how to extract a text from a document:


## get_text {#groupdocs.parser.options.TextOptions}

Extracts a text page from the document using text options (to enable raw fast text extraction mode).


### Returns 


An instance of TextReader class with the extracted text;
`null` if text extraction isn't supported.


```python
def get_text(self, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| options | groupdocs.parser.options.TextOptions | The text extraction options. |

### Example 


The following example shows how to extract a raw text from a document:


## get_text {#int}

Extracts a text from the document page.


### Returns 


An instance of TextReader class with the extracted text;
`null` if text page extraction isn't supported.


```python
def get_text(self, page_index):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| page_index | int | The zero-based page index. |

### Example 


The following example shows how to extract a text from the document page:


## get_text {#int-groupdocs.parser.options.TextOptions}

Extracts a text from the document page using text options (to enable raw fast text extraction mode).


### Returns 


An instance of TextReader class with the extracted text;
`null` if text page extraction isn't supported.


```python
def get_text(self, page_index, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| page_index | int | The zero-based page index. |
| options | groupdocs.parser.options.TextOptions | The text extraction options. |

### Example 


The following example shows how to extract a raw text from the document page:



### See Also
* module [`groupdocs.parser`](../../)
* class [`Parser`](/parser/python-net/groupdocs.parser/parser)

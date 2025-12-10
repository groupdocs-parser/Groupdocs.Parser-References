---
title: get_tables method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser/parser/get_tables/
is_root: false
weight: 140
---

## get_tables {#}

Extracts tables from the document.


### Returns 


A collection of [`PageTableArea`](/parser/python-net/groupdocs.parser.data/pagetablearea) objects;
`null` if tables extraction isn't supported.


```python
def get_tables(self):
    ...
```



### Example 


The following example shows how to extract tables from the whole document:


## get_tables {#groupdocs.parser.options.PageTableAreaOptions}

Extracts tables from the document.


### Returns 


A collection of [`PageTableArea`](/parser/python-net/groupdocs.parser.data/pagetablearea) objects;
`null` if tables extraction isn't supported.


```python
def get_tables(self, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| options | groupdocs.parser.options.PageTableAreaOptions | The options for tables extraction. |

### Example 


The following example shows how to extract tables from the whole document:


## get_tables {#int}

Extracts tables from the document page.


### Returns 


A collection of [`PageTableArea`](/parser/python-net/groupdocs.parser.data/pagetablearea) objects;
`null` if tables extraction isn't supported.


```python
def get_tables(self, page_index):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| page_index | int | The zero-based page index. |

### Example 


The following example shows how to extract tables from the document page:


## get_tables {#int-groupdocs.parser.options.PageTableAreaOptions}

Extracts tables from the document page.


### Returns 


A collection of [`PageTableArea`](/parser/python-net/groupdocs.parser.data/pagetablearea) objects;
`null` if tables extraction isn't supported.


```python
def get_tables(self, page_index, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| page_index | int | The zero-based page index. |
| options | groupdocs.parser.options.PageTableAreaOptions | The options for tables extraction. |

### Example 


The following example shows how to extract tables from the document page:



### See Also
* module [`groupdocs.parser`](../../)
* class [`PageTableArea`](/parser/python-net/groupdocs.parser.data/pagetablearea)
* class [`Parser`](/parser/python-net/groupdocs.parser/parser)

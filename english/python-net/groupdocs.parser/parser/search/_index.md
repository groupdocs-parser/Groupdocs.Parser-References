---
title: search method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser/parser/search/
is_root: false
weight: 230
---

## search {#System.String}

Searches a `keyword` in the document.


### Returns 


A collection of [`SearchResult`](/parser/python-net/groupdocs.parser.data/searchresult) objects; 
`null` if search isn't supported.


```python
def search(self, keyword):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| keyword | System.String | The keyword to search. |

### Example 


The following example shows how to find a keyword in a document:


## search {#System.String-groupdocs.parser.options.SearchOptions}

Searches a `keyword` in the document using search options (regular expression, match case, etc.).


### Returns 


A collection of [`SearchResult`](/parser/python-net/groupdocs.parser.data/searchresult) objects;
`null` if search isn't supported.


```python
def search(self, keyword, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| keyword | System.String | The keyword to search. |
| options | groupdocs.parser.options.SearchOptions | The search options. |

### Example 


The following example shows how to search with a regular expression in a document:


The following example shows how to search a text on pages:



### See Also
* module [`groupdocs.parser`](../../)
* class [`Parser`](/parser/python-net/groupdocs.parser/parser)
* class [`SearchResult`](/parser/python-net/groupdocs.parser.data/searchresult)

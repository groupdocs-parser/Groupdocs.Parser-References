---
title: get_formatted_text method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser/parser/get_formatted_text/
is_root: false
weight: 80
---

## get_formatted_text {#groupdocs.parser.options.FormattedTextOptions}

Extracts a formatted text from the document.


### Returns 


An instance of TextReader class with the extracted text;
`null` if formatted text extraction isn't supported.


```python
def get_formatted_text(self, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| options | groupdocs.parser.options.FormattedTextOptions | The formatted text extraction options. |

### Example 


The following example shows how to extract a document text as HTML text:


## get_formatted_text {#int-groupdocs.parser.options.FormattedTextOptions}

Extracts a formatted text from the document page.


### Returns 


An instance of TextReader class with the extracted text; 
`null` if formatted text page extraction isn't supported.


```python
def get_formatted_text(self, page_index, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| page_index | int | The zero-based page index. |
| options | groupdocs.parser.options.FormattedTextOptions | The formatted text extraction options. |

### Example 


The following example shows how to extract a document page text as Markdown text:



### See Also
* module [`groupdocs.parser`](../../)
* class [`Parser`](/parser/python-net/groupdocs.parser/parser)

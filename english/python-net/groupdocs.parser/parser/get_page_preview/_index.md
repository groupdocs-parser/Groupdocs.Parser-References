---
title: get_page_preview method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser/parser/get_page_preview/
is_root: false
weight: 130
---

## get_page_preview {#int}

Generates a document page preview.


### Returns 


An instance of Stream containing an image of the document page; `null` if the page preview generation isn't supported.


```python
def get_page_preview(self, page_index):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| page_index | int | The zero-based page index. |


## get_page_preview {#int-groupdocs.parser.options.PagePreviewOptions}

Generates a document page preview using customization options.


### Returns 


An instance of Stream containing an image of the document page; `null` if the page preview generation isn't supported.


```python
def get_page_preview(self, page_index, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| page_index | int | The zero-based page index. |
| options | groupdocs.parser.options.PagePreviewOptions | The options to customize the preview generation. |



### See Also
* module [`groupdocs.parser`](../../)
* class [`Parser`](/parser/python-net/groupdocs.parser/parser)

---
title: PreviewOptions constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.options/previewoptions/__init__/
is_root: false
weight: 10
---

## __init__ {#groupdocs.parser.options.ICreatePageStream}

Initializes a new instance of the [`PreviewOptions`](/parser/python-net/groupdocs.parser.options/previewoptions) class causing the output stream to be closed.



```python
def __init__(self, create_page_stream):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| create_page_stream | groupdocs.parser.options.ICreatePageStream | Creates a stream for a specific page preview. |


## __init__ {#groupdocs.parser.options.ICreatePageStream-groupdocs.parser.options.IReleasePageStream}

Initializes a new instance of [`PreviewOptions`](/parser/python-net/groupdocs.parser.options/previewoptions) class causing the output stream to be returned to the client for further use.



```python
def __init__(self, create_page_stream, release_page_stream):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| create_page_stream | groupdocs.parser.options.ICreatePageStream | Creates a stream for a specific page preview |
| release_page_stream | groupdocs.parser.options.IReleasePageStream | Notifies that the page preview generation is done and gets the output stream. |



### See Also
* module [`groupdocs.parser.options`](../../)
* class [`PreviewOptions`](/parser/python-net/groupdocs.parser.options/previewoptions)

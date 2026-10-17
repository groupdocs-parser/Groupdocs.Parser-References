---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new instance of the PreviewOptions class causing the output stream to be closed."
type: docs
url: /python-net/groupdocs.parser.options/previewoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#create_page_stream}

Initializes a new instance of the [`PreviewOptions`](/parser/python-net/groupdocs.parser.options/previewoptions/) class causing the output stream to be closed.

```python
def __init__(self, create_page_stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | Creates a stream for a specific page preview. |

## __init__ {#create_page_stream-release_page_stream}

Initializes a new instance of [`PreviewOptions`](/parser/python-net/groupdocs.parser.options/previewoptions/) causing the output stream to be returned to the client for further use.

```python
def __init__(self, create_page_stream, release_page_stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | Creates a stream for a specific page preview. |
| release_page_stream | `ReleasePageStream` | Notifies that the page preview generation is done and gets the output stream. |

### See Also
* class [`PreviewOptions`](/parser/python-net/groupdocs.parser.options/previewoptions/)

---
title: get_page_preview method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Generates a document page preview."
type: docs
url: /python-net/groupdocs.parser/parser/get_page_preview/
is_root: false
weight: 1310
---


## get_page_preview {#page_index}

Generates a document page preview.

```python
def get_page_preview(self, page_index):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| page_index | `int` | The zero-based page index. |

**Returns:** io.RawIOBase: An image of the document page; None if the page preview generation isn't supported.

## get_page_preview {#page_index-options}

Generates a document page preview using customization options.

```python
def get_page_preview(self, page_index, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| page_index | `int` | The zero-based page index. |
| options | `PagePreviewOptions` | The options to customize the preview generation. |

**Returns:** io.RawIOBase: A stream containing an image of the document page, or None if the page preview generation isn't supported.

### See Also
* class [`Parser`](/parser/python-net/groupdocs.parser/parser/)

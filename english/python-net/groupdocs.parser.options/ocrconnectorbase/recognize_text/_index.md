---
title: recognize_text method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Recognizes text from an image stream."
type: docs
url: /python-net/groupdocs.parser.options/ocrconnectorbase/recognize_text/
is_root: false
weight: 1010
---


## recognize_text {#image_stream-page_index-options}

Recognizes text from an image stream.

```python
def recognize_text(self, image_stream, page_index, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| image_stream | `io.RawIOBase` | The image representation of the document page. |
| page_index | `int` | The page index of the document. |
| options | `OcrOptions` | The OCR options. |

**Returns:** str | None: The recognized text, or None if text recognition isn't supported.

## recognize_text {#image_stream-options}

Recognize text from an image stream.

```python
def recognize_text(self, image_stream, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| image_stream | `io.RawIOBase` | The image representation of the document page. |
| options | `OcrOptions` | The OCR options. |

**Returns:** str or None: The recognized text, or None if text recognition isn’t supported.

### See Also
* class [`OcrConnectorBase`](/parser/python-net/groupdocs.parser.options/ocrconnectorbase/)

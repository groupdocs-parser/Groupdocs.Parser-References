---
title: recognize_text_areas method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Recognize text areas from image_stream stream."
type: docs
url: /python-net/groupdocs.parser.options/ocrconnectorbase/recognize_text_areas/
is_root: false
weight: 1020
---


## recognize_text_areas {#image_stream-page_index-page_size-options}

Recognize text areas from `image_stream` stream.

```python
def recognize_text_areas(self, image_stream, page_index, page_size, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| image_stream | `io.RawIOBase` | The image representation of the document page. |
| page_index | `int` | The page index of the document. |
| page_size | `Size` | The size of the document page. |
| options | `OcrOptions` | The OCR options. |

**Returns:** Iterable[PageTextArea]: A collection of PageTextArea objects; None if text areas recognizing isn't supported.

## recognize_text_areas {#image_stream-page_size-options}

Recognizes text areas from the provided image stream.

```python
def recognize_text_areas(self, image_stream, page_size, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| image_stream | `io.RawIOBase` | The image representation of the document page. |
| page_size | `Size` | The size of the document page. |
| options | `OcrOptions` | The OCR options. |

**Returns:** A collection of `PageTextArea` objects; None if text areas recognizing isn't supported.

## recognize_text_areas {#image_stream-page-options}

Recognizes text areas from `image_stream` stream.

```python
def recognize_text_areas(self, image_stream, page, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| image_stream | `io.RawIOBase` | The image representation of the document page. |
| page | `Page` | The document page. |
| options | `OcrOptions` | The OCR options. |

**Returns:** A collection of `PageTextArea` objects; `None` if text areas recognizing isn't supported.

## recognize_text_areas {#image_stream-rectangles-allowed_symbols-page-options}

Recognizes text areas from the given image stream.

```python
def recognize_text_areas(self, image_stream, rectangles, allowed_symbols, page, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| image_stream | `io.RawIOBase` | The image representation of the document page. |
| rectangles | `Iterable[Rectangle]` | The collection of rectangular areas that limits the OCR functionality. |
| allowed_symbols | `str` | The filter of allowed symbols by OCR. |
| page | `Page` | The document page. |
| options | `OcrOptions` | The OCR options. |

**Returns:** A collection of `PageTextArea` objects; `None` if text areas recognizing isn't supported.

### See Also
* class [`OcrConnectorBase`](/parser/python-net/groupdocs.parser.options/ocrconnectorbase/)

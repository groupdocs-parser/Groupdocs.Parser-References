---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new instance of the OcrOptions class with rectangular area."
type: docs
url: /python-net/groupdocs.parser.options/ocroptions/__init__/
is_root: false
weight: 10
---


## __init__

Initializes a new instance of the [`OcrOptions`](/parser/python-net/groupdocs.parser.options/ocroptions/) class with rectangular area.

```python
def __init__(self):
    ...
```

## __init__ {#page_preview_options}

Initializes a new OcrOptions instance with rectangular area.

```python
def __init__(self, page_preview_options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| page_preview_options | `PagePreviewOptions` | An instance of `OcrOptions.page_preview_options` that sets properties for the document page preview generation. |

## __init__ {#rectangle}

Initializes a new instance of the [`OcrOptions`](/parser/python-net/groupdocs.parser.options/ocroptions/) class with a rectangular area.

```python
def __init__(self, rectangle):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| rectangle | `Rectangle` | The rectangular area that constraints the page area which is used for text recognizing. |

## __init__ {#handler}

Initializes a new OcrOptions instance with an OcrEventHandler to catch OCR events.

```python
def __init__(self, handler):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| handler | `OcrEventHandler` | An instance of `OcrEventHandler` to catch OCR events. |

## __init__ {#rectangle-handler}

Initializes a new instance of the [`OcrOptions`](/parser/python-net/groupdocs.parser.options/ocroptions/) class with a rectangular area and an [`OcrEventHandler`](/parser/python-net/groupdocs.parser.options/ocreventhandler/) object.

```python
def __init__(self, rectangle, handler):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| rectangle | `Rectangle` | The rectangular area that constraints the page area which is used for text recognizing. |
| handler | `OcrEventHandler` | An instance of `OcrEventHandler` to catch OCR events. |

## __init__ {#rectangle-handler-page_preview_options-use_spell_cheker}

Initializes a new OcrOptions instance.

```python
def __init__(self, rectangle, handler, page_preview_options, use_spell_cheker):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| rectangle | `Rectangle` | The rectangular area that constraints the page area which is used for text recognizing. |
| handler | `OcrEventHandler` | An instance of `OcrEventHandler` to catch OCR events. |
| page_preview_options | `PagePreviewOptions` | An instance of `OcrOptions.page_preview_options` class that sets properties for the document page preview generation. |
| use_spell_cheker | `bool` | The value that indicates whether the spell checker is used. |

## __init__ {#rectangle-handler-page_preview_options-use_spell_cheker-language}

Initializes a new instance of OcrOptions.

```python
def __init__(self, rectangle, handler, page_preview_options, use_spell_cheker, language):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| rectangle | `Rectangle` | The rectangular area that constraints the page area which is used for text recognizing. |
| handler | `OcrEventHandler` | An instance of `OcrEventHandler` to catch OCR events. |
| page_preview_options | `PagePreviewOptions` | An instance of `OcrOptions.page_preview_options` class that sets properties for the document page preview generation. |
| use_spell_cheker | `bool` | The value that indicates whether the spell checker is used. |
| language | `Language` | The language used for OCR. |

### See Also
* class [`OcrOptions`](/parser/python-net/groupdocs.parser.options/ocroptions/)

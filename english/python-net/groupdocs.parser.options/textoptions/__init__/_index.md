---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new instance of the TextOptions class."
type: docs
url: /python-net/groupdocs.parser.options/textoptions/__init__/
is_root: false
weight: 10
---


## __init__

Initializes a new instance of the [`TextOptions`](/parser/python-net/groupdocs.parser.options/textoptions/) class.

```python
def __init__(self):
    ...
```

## __init__ {#use_raw_mode_if_possible}

Initializes a new TextOptions instance.

```python
def __init__(self, use_raw_mode_if_possible):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| use_raw_mode_if_possible | `bool` | Indicates whether raw mode is used. |

### Example

```python
from groupdocs.parser.options import TextOptions

options = TextOptions(use_raw_mode_if_possible=True)
```

## __init__ {#use_raw_mode_if_possible-use_ocr}

Initializes a new TextOptions instance with the OCR usage option.

```python
def __init__(self, use_raw_mode_if_possible, use_ocr):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| use_raw_mode_if_possible | `bool` | The value that indicates whether the raw mode is used. |
| use_ocr | `bool` | The value that indicates whether the OCR functionality is used to extract a text. |

## __init__ {#use_raw_mode_if_possible-use_ocr-ocr_options}

Initializes a new TextOptions instance with OCR options support.

```python
def __init__(self, use_raw_mode_if_possible, use_ocr, ocr_options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| use_raw_mode_if_possible | `bool` | Indicates whether raw mode is used. |
| use_ocr | `bool` | Indicates whether OCR functionality is used to extract text. |
| ocr_options | `OcrOptions` | Additional options for OCR functionality. |

### See Also
* class [`TextOptions`](/parser/python-net/groupdocs.parser.options/textoptions/)

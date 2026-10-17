---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new instance of the ParseByTemplateOptions class."
type: docs
url: /python-net/groupdocs.parser.options/parsebytemplateoptions/__init__/
is_root: false
weight: 10
---


## __init__

Initializes a new instance of the [`ParseByTemplateOptions`](/parser/python-net/groupdocs.parser.options/parsebytemplateoptions/) class.

```python
def __init__(self):
    ...
```

## __init__ {#page_index}

Initializes a new instance of the ParseByTemplateOptions class.

```python
def __init__(self, page_index):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| page_index | `int` | The page index. |

## __init__ {#page_index-use_ocr}

Initializes a new instance of the ParseByTemplateOptions class with the OCR usage option.

```python
def __init__(self, page_index, use_ocr):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| page_index | `int` | The page index. |
| use_ocr | `bool` | The value that indicates whether the OCR functionality is used to parse by template. |

## __init__ {#page_index-use_ocr-ocr_options}

Initializes a new instance of the [`ParseByTemplateOptions`](/parser/python-net/groupdocs.parser.options/parsebytemplateoptions/) class with the ability to set OCR options.

```python
def __init__(self, page_index, use_ocr, ocr_options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| page_index | `int` | The page index. |
| use_ocr | `bool` | The value that indicates whether the OCR functionality is used to parse by template. |
| ocr_options | `OcrOptions` | The additional options for OCR functionality. |

### See Also
* class [`ParseByTemplateOptions`](/parser/python-net/groupdocs.parser.options/parsebytemplateoptions/)

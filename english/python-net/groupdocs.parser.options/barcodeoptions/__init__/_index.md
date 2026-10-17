---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new instance of the BarcodeOptions class with default values."
type: docs
url: /python-net/groupdocs.parser.options/barcodeoptions/__init__/
is_root: false
weight: 10
---


## __init__

Initializes a new instance of the [`BarcodeOptions`](/parser/python-net/groupdocs.parser.options/barcodeoptions/) class with default values.

```python
def __init__(self):
    ...
```

## __init__ {#rectangle}

Initializes a new instance of the [`BarcodeOptions`](/parser/python-net/groupdocs.parser.options/barcodeoptions/) class with the rectangular area.

```python
def __init__(self, rectangle):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| rectangle | `Rectangle` | The rectangular area that contains barcodes. |

## __init__ {#image_quality-barcode_quality-code_types}

Initializes a new instance of the [`BarcodeOptions`](/parser/python-net/groupdocs.parser.options/barcodeoptions/) class with quality settings and code types.

```python
def __init__(self, image_quality, barcode_quality, code_types):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| image_quality | `QualityMode` | The quality of a source image. |
| barcode_quality | `QualityMode` | The quality of a source barcode. |
| code_types | `list[str]` | The types of barcodes to read. |

## __init__ {#rectangle-image_quality-barcode_quality-dimension-allow_incorrect_barcodes-code_types}

Initializes a new instance of the BarcodeOptions class.

```python
def __init__(self, rectangle, image_quality, barcode_quality, dimension, allow_incorrect_barcodes, code_types):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| rectangle | `Rectangle` | The rectangular area that contains barcodes. |
| image_quality | `QualityMode` | The quality of a source image. |
| barcode_quality | `QualityMode` | The quality of a source barcode. |
| dimension | `Optional[float]` | The minimal size of the barcode minimal element. |
| allow_incorrect_barcodes | `bool` | The value that indicates whether the incorrect barcodes are allowed. |
| code_types | `list[str]` | The types of barcodes to read. |

### See Also
* class [`BarcodeOptions`](/parser/python-net/groupdocs.parser.options/barcodeoptions/)

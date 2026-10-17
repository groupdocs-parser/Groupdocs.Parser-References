---
title: get_barcodes method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Extracts barcodes from the document."
type: docs
url: /python-net/groupdocs.parser/parser/get_barcodes/
is_root: false
weight: 1080
---


## get_barcodes

Extracts barcodes from the document.

```python
def get_barcodes(self):
    ...
```

**Returns:** A collection of `PageBarcodeArea` objects; `None` if barcodes extraction isn't supported.

### Example

```python
from groupdocs.parser import Parser

file_path = "sample.pdf"
with Parser(file_path) as parser:
    barcodes = parser.get_barcodes()
    for barcode in barcodes:
        print(f"Page: {barcode.page.index}")
        print(f"Value: {barcode.value}")
```

## get_barcodes {#page_index}

Extracts barcodes from the document page.

```python
def get_barcodes(self, page_index):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| page_index | `int` | The zero-based page index. |

**Returns:** Iterable[PageBarcodeArea] or None: A collection of `PageBarcodeArea` objects; `None` if barcodes extraction isn't supported.

### Example

```python
from groupdocs.parser import Parser

parser = Parser(file_path)
barcodes = parser.get_barcodes(1)
for barcode in barcodes:
    print(f"Page: {barcode.page.index}")
    print(f"Value: {barcode.value}")
```

## get_barcodes {#options}

Extracts barcodes from the document using customization options (to set the rectangular area that contains barcodes).

The following example shows how to extract barcodes from the upper‑right corner.

```python
def get_barcodes(self, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| options | `PageAreaOptions` | The options for barcodes extraction. |

**Returns:** list[PageBarcodeArea]: A collection of PageBarcodeArea objects; None if barcodes extraction isn't supported.

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.data import Rectangle, Point, Size
from groupdocs.parser.options import PageAreaOptions

with Parser(file_path) as parser:
    options = PageAreaOptions(Rectangle(Point(590, 80), Size(150, 150)))
    barcodes = parser.get_barcodes(options)
    for barcode in barcodes:
        print(f"Page: {barcode.page.index}")
        print(f"Value: {barcode.value}")
```

## get_barcodes {#options}

Extracts barcodes from the document using customization options.

```python
def get_barcodes(self, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| options | `BarcodeOptions` | The options for barcodes extraction. |

**Returns:** Iterable[PageBarcodeArea] | None: A collection of PageBarcodeArea objects; None if barcodes extraction isn't supported.

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.data import Rectangle, Point, Size
from groupdocs.parser.options import BarcodeOptions

file_path = "sample.pdf"
with Parser(file_path) as parser:
    # Extract barcodes from the upper‑right corner of each page
    options = BarcodeOptions(Rectangle(Point(590, 80), Size(150, 150)))
    barcodes = parser.get_barcodes(options)

    for barcode in barcodes:
        print(f"Page: {barcode.page.index}")
        print(f"Value: {barcode.value}")
```

## get_barcodes {#page_index-options}

Extracts barcodes from a document page using customization options to set the rectangular area that contains barcodes.

```python
def get_barcodes(self, page_index, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| page_index | `int` | The zero-based page index. |
| options | `PageAreaOptions` | The options for barcodes extraction. |

**Returns:** list[PageBarcodeArea] | None: A collection of PageBarcodeArea objects; None if barcode extraction isn't supported.

## get_barcodes {#page_index-options}

Extracts barcodes from the document page using customization options.

```python
def get_barcodes(self, page_index, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| page_index | `int` | The zero-based page index. |
| options | `BarcodeOptions` | The options for barcodes extraction. |

**Returns:** list[PageBarcodeArea] or None: A collection of PageBarcodeArea objects; None if barcode extraction isn't supported.

### See Also
* class [`Parser`](/parser/python-net/groupdocs.parser/parser/)

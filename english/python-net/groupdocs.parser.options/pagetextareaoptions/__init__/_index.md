---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new PageTextAreaOptions instance with the OCR usage option."
type: docs
url: /python-net/groupdocs.parser.options/pagetextareaoptions/__init__/
is_root: false
weight: 10
---


## __init__

Initializes a new PageTextAreaOptions instance with the OCR usage option.

```python
def __init__(self):
    ...
```

## __init__ {#use_ocr}

Initializes a new instance of the [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/) class with the OCR usage option.

```python
def __init__(self, use_ocr):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| use_ocr | `bool` | The value that indicates whether OCR functionality is used to extract text areas. |

## __init__ {#use_ocr-ocr_options}

Initializes a new instance of the PageTextAreaOptions class with the ability to set OCR options.

```python
def __init__(self, use_ocr, ocr_options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| use_ocr | `bool` | The value that indicates whether OCR functionality is used to extract text areas. |
| ocr_options | `OcrOptions` | The additional options for OCR functionality. |

## __init__ {#expression}

Initializes a new [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/) instance with the regular expression.

The following properties have default values:

- [`PageTextAreaOptions.MatchCase`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/match_case/): False
- [`PageTextAreaOptions.UniteSegments`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/unite_segments/): False
- [`PageTextAreaOptions.IgnoreFormatting`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/ignore_formatting/): False
- [`PageAreaOptions.Rectangle`](/parser/python-net/groupdocs.parser.data/rectangle/): None

```python
def __init__(self, expression):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| expression | `str` | The regular expression. |

### Example

```python
from groupdocs.parser.options import PageTextAreaOptions

options = PageTextAreaOptions(expression=r"\d{4}-\d{2}-\d{2}")
```

## __init__ {#expression-rectangle}

Initializes a new [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/) instance with the regular expression and rectangular area, leaving other options at their default values.

By default, `MatchCase`, `UniteSegments`, and `IgnoreFormatting` are set to `False`.

```python
def __init__(self, expression, rectangle):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| expression | `str` | The regular expression. |
| rectangle | `Rectangle` | The rectangular area that contains page areas. |

### Example

```python
from groupdocs.parser.options import PageTextAreaOptions
from groupdocs.parser.data import Rectangle, Point, Size

rect = Rectangle(Point(0, 0), Size(200, 100))
options = PageTextAreaOptions(r"\w+", rect)
```

## __init__ {#expression-rectangle-rectangle_tolerance}

Initializes a new instance of the PageTextAreaOptions class with the regular expression, rectangular area and the size of the ignored border.

```python
def __init__(self, expression, rectangle, rectangle_tolerance):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| expression | `str` | The regular expression. |
| rectangle | `Rectangle` | The rectangular area that contains page areas. |
| rectangle_tolerance | `float` | The size of the border that is ignored when captured by the rectangular area. Measured as a fraction of a text item height. |

### Example

```python
from groupdocs.parser.options import PageTextAreaOptions
from groupdocs.parser.data import Rectangle

options = PageTextAreaOptions(
    expression=r"\d+",
    rectangle=Rectangle(0, 0, 100, 200),
    rectangle_tolerance=0.1
)
```

## __init__ {#expression-match_case-unite_segments-ignore_formatting-rectangle}

Initializes a new PageTextAreaOptions instance.

```python
def __init__(self, expression, match_case, unite_segments, ignore_formatting, rectangle):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| expression | `str` | The regular expression. |
| match_case | `bool` | Indicates whether text case is considered. |
| unite_segments | `bool` | Indicates whether segments are united. |
| ignore_formatting | `bool` | Indicates whether text formatting is ignored. |
| rectangle | `Rectangle` | The rectangular area that contains page areas. |

### Example

```python
from groupdocs.parser.options import PageTextAreaOptions
from groupdocs.parser.data import Rectangle, Point, Size

# Define a rectangular region (x=0, y=0, width=200, height=100)
rect = Rectangle(Point(0, 0), Size(200, 100))

options = PageTextAreaOptions(
    expression=r"\d{4}-\d{2}-\d{2}",
    match_case=True,
    unite_segments=False,
    ignore_formatting=False,
    rectangle=rect,
)
```

## __init__ {#expression-match_case-unite_segments-ignore_formatting-rectangle-rectangle_tolerance}

Initializes a new PageTextAreaOptions instance with the size of the ignored border.

```python
def __init__(self, expression, match_case, unite_segments, ignore_formatting, rectangle, rectangle_tolerance):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| expression | `str` | The regular expression. |
| match_case | `bool` | Indicates whether text case is considered. |
| unite_segments | `bool` | Indicates whether segments are united. |
| ignore_formatting | `bool` | Indicates whether text formatting is ignored. |
| rectangle | `Rectangle` | The rectangular area that contains page areas. |
| rectangle_tolerance | `float` | The size of the border that is ignored when captured by the rectangular area. Measured as a fraction of a text item height. |

### Example

```python
from groupdocs.parser.options import PageTextAreaOptions
from groupdocs.parser.data import Rectangle

options = PageTextAreaOptions(
    expression=r"\d+",
    match_case=True,
    unite_segments=False,
    ignore_formatting=False,
    rectangle=Rectangle(0, 0, 100, 200),
    rectangle_tolerance=0.05,
)
```

### See Also
* class [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/)

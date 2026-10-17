---
title: get_text_areas method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Extracts text areas from the document."
type: docs
url: /python-net/groupdocs.parser/parser/get_text_areas/
is_root: false
weight: 1380
---


## get_text_areas

Extracts text areas from the document.

Learn more:
- Extract text areas (https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

```python
def get_text_areas(self):
    ...
```

**Returns:** list[PageTextArea] or None: A collection of `PageTextArea` objects; `None` if text areas extraction isn't supported.

### Example

```python
from groupdocs.parser import Parser

with Parser("./sample.pdf") as parser:
    # Extract text areas
    text_areas = parser.get_text_areas()
    if text_areas is None:
        print("Text areas extraction isn't supported")
    else:
        for area in text_areas:
            print(f"Page: {area.page.index}, R: {area.rectangle}, Text: {area.text}")
```

## get_text_areas {#options}

Extracts text areas from the document using customization options (regular expression, match case, etc.).

Learn more:
- https://docs.groupdocs.com/display/parsernet/Extract+text+areas

```python
def get_text_areas(self, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| options | `PageTextAreaOptions` | The options for text area extraction. |

**Returns:** list[PageTextArea] | None: A collection of `PageTextArea` objects; `None` if text areas extraction isn't supported.

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.data import Rectangle, Point, Size
from groupdocs.parser.options import PageTextAreaOptions

with Parser("./sample.pdf") as parser:
    region = Rectangle(Point(0, 0), Size(300, 100))
    options = PageTextAreaOptions(r"\d+", region)
    text_areas = parser.get_text_areas(options)
    if text_areas is None:
        print("Text areas extraction isn't supported")
    else:
        for area in text_areas:
            print(f"Page: {area.page.index}, R: {area.rectangle}, Text: {area.text}")
```

## get_text_areas {#page_index}

Extracts text areas from the document page.

Learn more:
- Extract text areas

```python
def get_text_areas(self, page_index):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| page_index | `int` | The zero-based page index. |

**Returns:** list[PageTextArea] | None: A collection of PageTextArea objects; None if text areas extraction isn't supported.

### Example

```python
from groupdocs.parser import Parser

with Parser("./sample.docx") as parser:
    # Verify that the document supports text areas extraction
    if parser.features.text_areas:
        # Extract text areas from the first page (page index 0)
        text_areas = parser.get_text_areas(0)
        if text_areas is None:
            print("Text areas extraction isn't supported")
        else:
            for area in text_areas:
                print(f"Rectangle: {area.rectangle}, Text: {area.text}")
```

## get_text_areas {#page_index-options}

Extracts text areas from the document page using customization options (regular expression, match case, etc.).

Learn more:

- https://docs.groupdocs.com/display/parsernet/Extract+text+areas

```python
def get_text_areas(self, page_index, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| page_index | `int` | The zero-based page index. |
| options | `PageTextAreaOptions` | The options for text area extraction. |

**Returns:** list[PageTextArea] or None: A collection of PageTextArea objects; None if text areas extraction isn't supported.

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import PageTextAreaOptions

with Parser("./sample.docx") as parser:
    text_areas = parser.get_text_areas()
    if text_areas is None:
        print("Text areas extraction isn't supported")
    else:
        for area in text_areas:
            if area.text_style is not None:
                print(f"Text: {area.text}")
```

### See Also
* class [`Parser`](/parser/python-net/groupdocs.parser/parser/)

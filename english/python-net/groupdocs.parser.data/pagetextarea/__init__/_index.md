---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new PageTextArea instance."
type: docs
url: /python-net/groupdocs.parser.data/pagetextarea/__init__/
is_root: false
weight: 10
---


## __init__ {#text-page-rectangle}

Initializes a new PageTextArea instance.

```python
def __init__(self, text, page, rectangle):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| text | `str` | The value of the text. |
| page | `Page` | The page that contains the text area. |
| rectangle | `Rectangle` | The rectangular area that contains the text area. |

## __init__ {#text-base_line-text_style-page-rectangle}

Initializes a new PageTextArea.

```python
def __init__(self, text, base_line, text_style, page, rectangle):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| text | `str` | The value of the text. |
| base_line | `Optional[float]` | The base line of the text. |
| text_style | `TextStyle` | The style of the text. |
| page | `Page` | The page that contains the text area. |
| rectangle | `Rectangle` | The rectangular area that contains the text area. |

## __init__ {#areas-page}

Initializes a new PageTextArea instance.

```python
def __init__(self, areas, page):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| areas | `Iterable[PageTextArea]` | The collection of child text page areas. |
| page | `Page` | The page that contains the text area. |

### See Also
* class [`PageTextArea`](/parser/python-net/groupdocs.parser.data/pagetextarea/)

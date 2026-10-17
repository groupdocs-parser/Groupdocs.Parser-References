---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new instance of the HighlightOptions class which is used to extract a fixed-length highlight."
type: docs
url: /python-net/groupdocs.parser.options/highlightoptions/__init__/
is_root: false
weight: 10
---


## __init__

Initializes a new instance of the [`HighlightOptions`](/parser/python-net/groupdocs.parser.options/highlightoptions/) class which is used to extract a fixed-length highlight.

```python
def __init__(self):
    ...
```

## __init__ {#max_length}

Initializes a new HighlightOptions instance used to extract a fixed-length highlight.

```python
def __init__(self, max_length):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| max_length | `int` | The maximum text length. |

## __init__ {#max_length-is_line_limited}

Initializes a new instance of the [`HighlightOptions`](/parser/python-net/groupdocs.parser.options/highlightoptions/) class which is used to extract a line‑limited highlight.

```python
def __init__(self, max_length, is_line_limited):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| max_length | `Optional[int]` | The maximum text length. |
| is_line_limited | `bool` | Indicates whether the highlight extraction is limited by the start (or the end) of a text line. |

### Example

```python
from groupdocs.parser.options import HighlightOptions

# Create options to extract a highlight with a maximum length of 200 characters,
# limiting the highlight to the start/end of a line.
options = HighlightOptions(max_length=200, is_line_limited=True)
```

## __init__ {#max_length-word_count}

Initializes a new HighlightOptions instance used to extract a highlight with a fixed word count.

```python
def __init__(self, max_length, word_count):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| max_length | `Optional[int]` | The maximum text length. |
| word_count | `int` | The maximum word count. |

## __init__ {#max_length-word_count-is_line_limited}

Initializes a new HighlightOptions instance.

```python
def __init__(self, max_length, word_count, is_line_limited):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| max_length | `Optional[int]` | The maximum text length. |
| word_count | `Optional[int]` | The maximum word count. |
| is_line_limited | `bool` | The value that indicates whether the highlight extraction is limited by the start (or the end) of a text line. |

### See Also
* class [`HighlightOptions`](/parser/python-net/groupdocs.parser.options/highlightoptions/)

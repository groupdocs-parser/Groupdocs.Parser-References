---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new instance of the FormattedTextOptions class."
type: docs
url: /python-net/groupdocs.parser.options/formattedtextoptions/__init__/
is_root: false
weight: 10
---


## __init__

Initializes a new instance of the [`FormattedTextOptions`](/parser/python-net/groupdocs.parser.options/formattedtextoptions/) class.

```python
def __init__(self):
    ...
```

### Example

```python
from groupdocs.parser.options import FormattedTextOptions, FormattedTextMode

options = FormattedTextOptions(FormattedTextMode.MARKDOWN)
```

## __init__ {#mode}

Initializes a new FormattedTextOptions instance.

```python
def __init__(self, mode):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| mode | `FormattedTextMode` | The mode of formatted text extraction. |

### Example

```python
    from groupdocs.parser import Parser
    from groupdocs.parser.options import FormattedTextOptions, FormattedTextMode

    with Parser("sample.pptx") as parser:
        reader = parser.get_formatted_text(
            FormattedTextOptions(FormattedTextMode.MARKDOWN)
        )
        print(reader.read_to_end() if reader is not None else "Formatted text isn't available.")
    ```

### See Also
* class [`FormattedTextOptions`](/parser/python-net/groupdocs.parser.options/formattedtextoptions/)

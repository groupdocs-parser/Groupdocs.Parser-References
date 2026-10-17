---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new instance of the ImageOptions class."
type: docs
url: /python-net/groupdocs.parser.options/imageoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#image_format}

Initializes a new instance of the [`ImageOptions`](/parser/python-net/groupdocs.parser.options/imageoptions/) class.

```python
def __init__(self, image_format):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| image_format | `ImageFormat` | The format of the image. |

### Example

```python
from groupdocs.parser.options import ImageOptions, ImageFormat

# Create options to extract images as JPEG
options = ImageOptions(image_format=ImageFormat.JPEG)
```

### See Also
* class [`ImageOptions`](/parser/python-net/groupdocs.parser.options/imageoptions/)

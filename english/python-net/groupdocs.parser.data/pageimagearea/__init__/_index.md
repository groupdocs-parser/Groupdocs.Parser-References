---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new instance of the PageImageArea class."
type: docs
url: /python-net/groupdocs.parser.data/pageimagearea/__init__/
is_root: false
weight: 10
---


## __init__ {#image_stream-file_type-rotation}

Initializes a new instance of the [`PageImageArea`](/parser/python-net/groupdocs.parser.data/pageimagearea/) class.

```python
def __init__(self, image_stream, file_type, rotation):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| image_stream | `io.RawIOBase` | The stream of the image. |
| file_type | `FileType` | The format of the image. |
| rotation | `float` | The rotation angle of the image. |

## __init__ {#image_stream-file_type-rotation-page-rectangle}

Initializes a new PageImageArea instance.

```python
def __init__(self, image_stream, file_type, rotation, page, rectangle):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| image_stream | `io.RawIOBase` | The stream of the image. |
| file_type | `FileType` | The format of the image. |
| rotation | `float` | The rotation angle of the image. |
| page | `Page` | The page that contains the image. |
| rectangle | `Rectangle` | The rectangular area that contains the image. |

### Example

```python
from groupdocs.parser.data import PageImageArea, Page, Rectangle
from groupdocs.parser.options import FileType

# Assume `page_obj` is a `Page` instance obtained from a parsed document
with open("image.png", "rb") as stream:
    area = PageImageArea(
        image_stream=stream,
        file_type=FileType.PNG,
        rotation=0.0,
        page=page_obj,
        rectangle=Rectangle(0, 0, 100, 100)
    )
    # Save the extracted image to a file
    area.save("output.png")
```

### See Also
* class [`PageImageArea`](/parser/python-net/groupdocs.parser.data/pageimagearea/)

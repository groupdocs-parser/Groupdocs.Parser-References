---
title: save method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Saves the image to the file."
type: docs
url: /python-net/groupdocs.parser.data/pageimagearea/save/
is_root: false
weight: 1030
---


## save {#file_path}

Saves the image to the file.

```python
def save(self, file_path):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | The path to the file. |

### Example

```python
import uuid
from groupdocs.parser import Parser

parser = Parser(file_path)
images = parser.get_images()

if images is None:
    print("Page images extraction isn't supported")
else:
    for image in images:
        # Save the image to a file with a unique name
        image.save(f"{uuid.uuid4()}{image.file_type.extension}")
```

## save {#file_path-options}

Saves the image to the file in a different format.

```python
def save(self, file_path, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | The path to the file. |
| options | `ImageOptions` | The options which are used to save the image. |

### Example

```python
import uuid
from groupdocs.parser import Parser
from groupdocs.parser.options import ImageOptions, ImageFormat

# Initialize parser for the source document
parser = Parser(file_path)

# Extract images from the document
images = parser.get_images()

if images is None:
    print("Page images extraction isn't supported")
else:
    # Create options to save images in PNG format
    options = ImageOptions(ImageFormat.Png)

    for image in images:
        # Save each image to a PNG file with a unique name
        image.save(f"{uuid.uuid4()}.png", options)
```

### See Also
* class [`PageImageArea`](/parser/python-net/groupdocs.parser.data/pageimagearea/)

---
title: get_image_stream method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Returns the image stream."
type: docs
url: /python-net/groupdocs.parser.data/pageimagearea/get_image_stream/
is_root: false
weight: 1010
---


## get_image_stream

Returns the image stream.

```python
def get_image_stream(self):
    ...
```

**Returns:** A stream with the image.

### Example

```python
from groupdocs.parser import Parser

with Parser("brochure.pdf") as parser:
    images = parser.get_images()
    if images is None:
        print("Image extraction isn't supported for this format.")
    elif not images:
        print("No images found")
    else:
        for image_area in images:
            # The image stream is a .NET MemoryStream; to_array() returns its bytes
            with image_area.get_image_stream() as stream:
                data = stream.to_array()
                print(f"Read {len(data)} bytes from page {image_area.page.index + 1}")
```

## get_image_stream {#options}

Returns the image stream in a different format.

```python
def get_image_stream(self, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| options | `ImageOptions` | The options which are used to extract the image. |

**Returns:** io.RawIOBase: A stream with the image.

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import ImageOptions, ImageFormat

with Parser("document.pdf") as parser:
    images = parser.get_images()
    if not images:
        print("No images found or extraction not supported.")
    else:
        options = ImageOptions(ImageFormat.Png)
        for area in images:
            # The image stream is a .NET MemoryStream; to_array() returns its bytes
            with area.get_image_stream(options) as stream:
                data = stream.to_array()
                # Save the image to a file
                file_name = f"page_{area.page.index + 1}.png"
                with open(file_name, "wb") as f:
                    f.write(data)
                print(f"Saved {len(data)} bytes to {file_name}")
```

### See Also
* class [`PageImageArea`](/parser/python-net/groupdocs.parser.data/pageimagearea/)

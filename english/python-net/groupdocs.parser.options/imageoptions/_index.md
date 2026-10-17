---
title: ImageOptions class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Provides options used for image extraction."
type: docs
url: /python-net/groupdocs.parser.options/imageoptions/
is_root: false
weight: 220
---


## ImageOptions class

Provides options used for image extraction.

An instance of [`ImageOptions`](/parser/python-net/groupdocs.parser.options/imageoptions/) is used as a parameter in `PageImageArea.get_image_stream(ImageOptions)` and `PageImageArea.save(str, ImageOptions)` methods. See the usage examples there.

It is used to specify the image format for image extraction.

- https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area
- https://docs.groupdocs.com/display/parsernet/Extract+images+to+files

The ImageOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.options/imageoptions/__init__/#image_format) | Initializes a new instance of the [`ImageOptions`](/parser/python-net/groupdocs.parser.options/imageoptions/) class. |

### Properties
| Property | Description |
| :- | :- |
| [image_format](/parser/python-net/groupdocs.parser.options/imageoptions/image_format/) | The image format for image extraction. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import ImageOptions, ImageFormat

parser = Parser("sample.docx")
image_area = parser.get_images()[0]

# Save images as JPEG
options = ImageOptions(ImageFormat.JPEG)

# Retrieve the image as a stream
stream = image_area.get_image_stream(options)

# Or save the image directly to a file
image_area.save("output.jpg", options)
```

### See Also
* module [`groupdocs.parser.options`](/parser/python-net/groupdocs.parser.options/)

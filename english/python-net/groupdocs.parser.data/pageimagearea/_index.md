---
title: PageImageArea class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Represents a page image area used to represent an image on a page in template parsing or an image attachment extracted from emails or Zip archives."
type: docs
url: /python-net/groupdocs.parser.data/pageimagearea/
is_root: false
weight: 130
---


## PageImageArea class

Represents a page image area used to represent an image on a page in template parsing or an image attachment extracted from emails or Zip archives.

An instance of [`PageImageArea`](/parser/python-net/groupdocs.parser.data/pageimagearea/) is returned by the following methods:

- [`Parser.get_images`](/parser/python-net/groupdocs.parser/parser/get_images/)
- [`Parser.get_images`](/parser/python-net/groupdocs.parser/parser/get_images/)
- [`Parser.get_images`](/parser/python-net/groupdocs.parser/parser/get_images/)
- [`Parser.get_images`](/parser/python-net/groupdocs.parser/parser/get_images/)

See the usage examples there.

The PageImageArea type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.data/pageimagearea/__init__/#image_stream-file_type-rotation) | Initializes a new instance of the [`PageImageArea`](/parser/python-net/groupdocs.parser.data/pageimagearea/) class. |
| [__init__](/parser/python-net/groupdocs.parser.data/pageimagearea/__init__/#image_stream-file_type-rotation-page-rectangle) | Initializes a new PageImageArea instance. |

### Methods
| Method | Description |
| :- | :- |
| [get_image_stream](/parser/python-net/groupdocs.parser.data/pageimagearea/get_image_stream/) | Returns the image stream. |
| [get_image_stream](/parser/python-net/groupdocs.parser.data/pageimagearea/get_image_stream/#options) | Returns the image stream in a different format. |
| [get_image_stream_image_options](/parser/python-net/groupdocs.parser.data/pageimagearea/get_image_stream_image_options/) |  |
| [save](/parser/python-net/groupdocs.parser.data/pageimagearea/save/#file_path) | Saves the image to the file. |
| [save](/parser/python-net/groupdocs.parser.data/pageimagearea/save/#file_path-options) | Saves the image to the file in a different format. |
| [save_file](/parser/python-net/groupdocs.parser.data/pageimagearea/save_file/) |  |
| [save_string](/parser/python-net/groupdocs.parser.data/pageimagearea/save_string/) |  |

### Properties
| Property | Description |
| :- | :- |
| [file_type](/parser/python-net/groupdocs.parser.data/pageimagearea/file_type/) | The format of the image as a [`FileType`](/parser/python-net/groupdocs.parser.options/filetype/) instance. |
| [rotation](/parser/python-net/groupdocs.parser.data/pageimagearea/rotation/) | The rotation angle of the image. |
| [page](/parser/python-net/groupdocs.parser.data/pagearea/page/) | The document page information such as page index and page size. (inherited from [`PageArea`](/parser/python-net/groupdocs.parser.data/pagearea/)) |
| [rectangle](/parser/python-net/groupdocs.parser.data/pagearea/rectangle/) | The rectangular area of the page as a [`Rectangle`](/parser/python-net/groupdocs.parser.data/rectangle/). (inherited from [`PageArea`](/parser/python-net/groupdocs.parser.data/pagearea/)) |

### Example

```python
from groupdocs.parser import Parser

parser = Parser("sample.docx")
# Iterate over image areas on each page
for img_area in parser.get_images():
    # Save each image to a file; the page number can be used in the filename
    img_area.save(f"output/image_page_{img_area.page}.png")
```

### See Also
* module [`groupdocs.parser.data`](/parser/python-net/groupdocs.parser.data/)

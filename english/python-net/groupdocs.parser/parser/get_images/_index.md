---
title: get_images method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Extracts images from the document."
type: docs
url: /python-net/groupdocs.parser/parser/get_images/
is_root: false
weight: 1120
---


## get_images

Extracts images from the document.

Learn more:
- [Extract images from documents](https://docs.groupdocs.com/parser/python-net/extract-images-from-documents/)
- [Extract images to files](https://docs.groupdocs.com/parser/python-net/extract-images-to-files/)

```python
def get_images(self):
    ...
```

**Returns:** Iterable[PageImageArea]: A collection of `PageImageArea` objects; `None` if images extraction isn't supported.

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

## get_images {#options}

Extracts images from the document using customization options (to set the rectangular area that contains images).

Learn more:
- https://docs.groupdocs.com/parser/python-net/extract-images-from-documents/
- https://docs.groupdocs.com/parser/python-net/extract-images-to-files/
- https://docs.groupdocs.com/parser/python-net/extract-images-from-document-page-area/

```python
def get_images(self, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| options | `PageAreaOptions` | The options for images extraction. |

**Returns:** A collection of `PageImageArea` objects; None if images extraction isn't supported.

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
            with image_area.get_image_stream() as stream:
                data = stream.to_array()
                print(f"Read {len(data)} bytes from page {image_area.page.index + 1}")
```

## get_images {#page_index}

Extracts images from the document page.

```python
def get_images(self, page_index):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| page_index | `int` | The zero-based page index. |

**Returns:** list[PageImageArea] | None: A collection of `PageImageArea` objects; `None` if images extraction isn't supported.

### Example

```python
from groupdocs.parser import Parser

with Parser("brochure.pdf") as parser:
    images = parser.get_images(0)  # extract images from the first page
    if images is None:
        print("Image extraction isn't supported for this format.")
    elif not images:
        print("No images found")
    else:
        for image_area in images:
            with image_area.get_image_stream() as stream:
                data = stream.to_array()
                print(f"Read {len(data)} bytes from page {image_area.page.index + 1}")
```

## get_images {#page_index-options}

Extracts images from the document page using customization options (to set the rectangular area that contains images).

Learn more:
- [Extract images from documents](https://docs.groupdocs.com/parser/python-net/extract-images-from-documents/)
- [Extract images to files](https://docs.groupdocs.com/parser/python-net/extract-images-to-files/)
- [Extract images from document page](https://docs.groupdocs.com/parser/python-net/extract-images-from-document-page/)
- [Extract images from document page area](https://docs.groupdocs.com/parser/python-net/extract-images-from-document-page-area/)

```python
def get_images(self, page_index, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| page_index | `int` | The zero-based page index. |
| options | `PageAreaOptions` | The options for images extraction. |

**Returns:** list[PageImageArea] | None: A collection of `PageImageArea` objects; None if images extraction isn't supported.

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
            with image_area.get_image_stream() as stream:
                data = stream.to_array()
                print(f"Read {len(data)} bytes from page {image_area.page.index + 1}")
```

### Aliases

These names call `get_images` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_images_int32` | `get_images_int32(page_index, options)`<br>`get_images_int32(page_index)` |
| `get_images_page_area_options` | `get_images_page_area_options(options)` |

### See Also
* class [`Parser`](/parser/python-net/groupdocs.parser/parser/)

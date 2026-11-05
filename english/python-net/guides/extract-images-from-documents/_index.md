---
title: Extract Images from Documents
linkTitle: "Extract Images from Documents"
second_title: GroupDocs.Parser for Python via .NET API References
description: "Extract embedded images from PDF, Word, Excel, presentations, emails, and archives using GroupDocs.Parser for Python via .NET."
type: docs
url: /python-net/guides/extract-images-from-documents/
is_root: false
weight: 70
---


GroupDocs.Parser can list and export images from supported documents (PDF, Office, emails, eBooks, and more).

## Extract images
{{< tabs "example-1" >}}
{{< tab "Python" >}}

```python
from groupdocs.parser import Parser

with Parser("./slides.pptx") as parser:
    images = parser.get_images()
    if images is None:
        print("Image extraction isn't supported for this format.")
    else:
        print(f"Found {len(images)} images")
        for index, image_area in enumerate(images, start=1):
            print(f"Page: {image_area.page.index + 1}, Type: {image_area.file_type.file_format}")
            # Save each image (the extension includes the dot, e.g. ".png")
            output_path = f"image-{index}{image_area.file_type.extension}"
            image_area.save(output_path)
```

{{< /tab >}}
{{< tab "slides.pptx" >}}

The following sample file is used in this example: [slides.pptx](https://docs.groupdocs.com/parser/python-net/_sample_files/developer-guide/basic-usage/extract-images-from-documents/slides.pptx)

{{< /tab >}}
{{< tab "extract-images-outputs.zip" >}}  
```text
image-1.png (4 KB)
image-2.jpeg (136 KB)
image-3.jpeg (75 KB)
image-4.jpeg (105 KB)
```
[Download full output](https://docs.groupdocs.com/parser/python-net/_output_files/developer-guide/basic-usage/extract-images-from-documents/example-1/extract-images-outputs.zip)
{{< /tab >}}
{{< /tabs >}}

### Steps

1. Create [`Parser`](/parser/python-net/groupdocs.parser/parser/) for the source file.  
2. Call `get_images()` to obtain [`PageImageArea`](/parser/python-net/groupdocs.parser.data/pageimagearea/) items.  
3. Inspect `page`, `rectangle`, `file_type`, and save streams with `save()` or `get_image_stream()`.

For coordinates-based processing and format conversion, see the [advanced images guide](https://docs.groupdocs.com/parser/python-net/developer-guide/advanced-usage/working-with-images/); the same workflow applies in Python.

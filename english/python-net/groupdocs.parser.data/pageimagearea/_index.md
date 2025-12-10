---
title: PageImageArea class
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.data/pageimagearea/
is_root: false
weight: 120
---

## PageImageArea class

Represents a page image area which is used to represent an image on the page in the parsing by template functionality
or an image attachment if images are extracted from emails or Zip archives.



**Inheritance:** [`PageImageArea`](/parser/python-net/groupdocs.parser.data/pageimagearea) → 
[`PageArea`](/parser/python-net/groupdocs.parser.data/pagearea)



The PageImageArea type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.data/pageimagearea/__init__/#io.RawIOBase-groupdocs.parser.options.FileType-float) | Initializes a new instance of the [`PageImageArea`](/parser/python-net/groupdocs.parser.data/pageimagearea) class. |
| [__init__](/parser/python-net/groupdocs.parser.data/pageimagearea/__init__/#io.RawIOBase-groupdocs.parser.options.FileType-float-groupdocs.parser.data.Page-groupdocs.parser.data.Rectangle) | Initializes a new instance of the [`PageImageArea`](/parser/python-net/groupdocs.parser.data/pageimagearea) class. |


### Properties
| Property | Description |
| :- | :- |
| [rectangle](/parser/python-net/groupdocs.parser.data/pageimagearea/rectangle) | Gets the rectangular area. |
| [page](/parser/python-net/groupdocs.parser.data/pageimagearea/page) | Gets the document page information such as page index and page size. |
| [file_type](/parser/python-net/groupdocs.parser.data/pageimagearea/file_type) | Gets the format of the image. |
| [rotation](/parser/python-net/groupdocs.parser.data/pageimagearea/rotation) | Gets the rotation angle of the image. |


### Methods
| Method | Description |
| :- | :- |
| [get_image_stream](/parser/python-net/groupdocs.parser.data/pageimagearea/get_image_stream/#) | Returns the image stream. |
| [get_image_stream](/parser/python-net/groupdocs.parser.data/pageimagearea/get_image_stream/#groupdocs.parser.options.ImageOptions) | Returns the image stream in a different format. |
| [save](/parser/python-net/groupdocs.parser.data/pageimagearea/save/#System.String) | Saves the image to the file. |
| [save](/parser/python-net/groupdocs.parser.data/pageimagearea/save/#System.String-groupdocs.parser.options.ImageOptions) | Saves the image to the file in a different format. |



### Remarks 


An instance of [`PageImageArea`](/parser/python-net/groupdocs.parser.data/pageimagearea) class is used as return value
of the following methods:

|
|
 |
 |
 |
 |


See the usage examples there.

### See Also
* module [`groupdocs.parser.data`](..)
* class [`PageArea`](/parser/python-net/groupdocs.parser.data/pagearea)
* class [`PageImageArea`](/parser/python-net/groupdocs.parser.data/pageimagearea)

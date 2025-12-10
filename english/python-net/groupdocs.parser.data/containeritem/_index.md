---
title: ContainerItem class
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.data/containeritem/
is_root: false
weight: 10
---

## ContainerItem class

Represents a container item like Zip archive entity, email attachment, PDF Portfolio item and so on.



The ContainerItem type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [name](/parser/python-net/groupdocs.parser.data/containeritem/name) | Gets the name of the item. |
| [directory](/parser/python-net/groupdocs.parser.data/containeritem/directory) | Gets the directory of the item. |
| [file_path](/parser/python-net/groupdocs.parser.data/containeritem/file_path) | Gets the full path of the item. |
| [size](/parser/python-net/groupdocs.parser.data/containeritem/size) | Gets the size of the item. |
| [metadata](/parser/python-net/groupdocs.parser.data/containeritem/metadata) | Gets the collection of metadata items. |


### Methods
| Method | Description |
| :- | :- |
| [open_parser](/parser/python-net/groupdocs.parser.data/containeritem/open_parser/#) | Creates the [`Parser`](/parser/python-net/groupdocs.parser/parser) object for the item content. |
| [open_parser](/parser/python-net/groupdocs.parser.data/containeritem/open_parser/#groupdocs.parser.options.LoadOptions) | Creates the [`Parser`](/parser/python-net/groupdocs.parser/parser) object for the item content with [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions). |
| [open_parser](/parser/python-net/groupdocs.parser.data/containeritem/open_parser/#groupdocs.parser.options.LoadOptions-groupdocs.parser.options.ParserSettings) | Creates the [`Parser`](/parser/python-net/groupdocs.parser/parser) object for the item content with [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions)<br/>and [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings). |
| [get_metadata_value](/parser/python-net/groupdocs.parser.data/containeritem/get_metadata_value/#System.String) | Gets the metadata value. |
| [open_stream](/parser/python-net/groupdocs.parser.data/containeritem/open_stream/#) | Opens the stream of the item content. |
| [detect_file_type](/parser/python-net/groupdocs.parser.data/containeritem/detect_file_type/#groupdocs.parser.options.FileTypeDetectionMode) | Detects a file type of the container item. |



### Remarks 


An instance of [`ContainerItem`](/parser/python-net/groupdocs.parser.data/containeritem) class is used as return value
of [`Parser.get_container`](/parser/python-net/groupdocs.parser/parser/get_container) method. See the usage examples there.

### See Also
* module [`groupdocs.parser.data`](..)
* class [`ContainerItem`](/parser/python-net/groupdocs.parser.data/containeritem)
* class [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions)
* class [`Parser`](/parser/python-net/groupdocs.parser/parser)
* class [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings)

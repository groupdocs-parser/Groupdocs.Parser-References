---
title: ContainerItem class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Represents a container item like Zip archive entity, email attachment, PDF Portfolio item and so on."
type: docs
url: /python-net/groupdocs.parser.data/containeritem/
is_root: false
weight: 20
---


## ContainerItem class

Represents a container item like Zip archive entity, email attachment, PDF Portfolio item and so on.

An instance of [`ContainerItem`](/parser/python-net/groupdocs.parser.data/containeritem/) is used as the return value of [`Parser.get_container`](/parser/python-net/groupdocs.parser/parser/get_container/). See the usage examples there.

The ContainerItem type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [detect_file_type](/parser/python-net/groupdocs.parser.data/containeritem/detect_file_type/#detection_mode) | Detects the file type of the container item. |
| [detect_file_type_file_type_detection_mode](/parser/python-net/groupdocs.parser.data/containeritem/detect_file_type_file_type_detection_mode/) |  |
| [get_metadata_value](/parser/python-net/groupdocs.parser.data/containeritem/get_metadata_value/#name) | Gets the metadata value. |
| [get_metadata_value_file](/parser/python-net/groupdocs.parser.data/containeritem/get_metadata_value_file/) |  |
| [get_metadata_value_string](/parser/python-net/groupdocs.parser.data/containeritem/get_metadata_value_string/) |  |
| [open_parser](/parser/python-net/groupdocs.parser.data/containeritem/open_parser/) | Creates the [`Parser`](/parser/python-net/groupdocs.parser/parser/) object for the item content. |
| [open_parser](/parser/python-net/groupdocs.parser.data/containeritem/open_parser/#load_options) | Creates a [`Parser`](/parser/python-net/groupdocs.parser/parser/) object for the item content with [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions/). |
| [open_parser](/parser/python-net/groupdocs.parser.data/containeritem/open_parser/#load_options-parser_settings) | Creates a [`Parser`](/parser/python-net/groupdocs.parser/parser/) object for the item content with [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions/) and [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings/). |
| [open_parser_load_options](/parser/python-net/groupdocs.parser.data/containeritem/open_parser_load_options/) |  |
| [open_stream](/parser/python-net/groupdocs.parser.data/containeritem/open_stream/) | Opens the stream of the item content. |

### Properties
| Property | Description |
| :- | :- |
| [directory](/parser/python-net/groupdocs.parser.data/containeritem/directory/) | The directory of the item (without a file name). |
| [file_path](/parser/python-net/groupdocs.parser.data/containeritem/file_path/) | The full path of the item as a string. |
| [metadata](/parser/python-net/groupdocs.parser.data/containeritem/metadata/) | The collection of metadata items. |
| [name](/parser/python-net/groupdocs.parser.data/containeritem/name/) | The name of the item, a string representing the file name without a directory. |
| [size](/parser/python-net/groupdocs.parser.data/containeritem/size/) | The size of the item in bytes. |

### See Also
* module [`groupdocs.parser.data`](/parser/python-net/groupdocs.parser.data/)

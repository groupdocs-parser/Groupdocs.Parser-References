---
title: Parser class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Represents the main class that controls text, images, container extraction and parsing functionality."
type: docs
url: /python-net/groupdocs.parser/parser/
is_root: false
weight: 30
---


## Parser class

Represents the main class that controls text, images, container extraction and parsing functionality.

The Parser type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#uri) | Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser/) class to extract data from a URI. |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#uri-load_options) | Initializes a new Parser instance to extract data from a URI with the specified load options. |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#uri-parser_settings) | Initializes a new Parser to extract data from a URI using the specified parser settings. |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#uri-load_options-parser_settings) | Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser/) class to extract data from a URI with the specified load options and parser settings. |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#connection) | Initializes a new Parser instance to extract data from a database. |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#connection-parser_settings) | Initializes a new Parser instance to extract data from a database. |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#connection) | Initializes a new Parser instance to extract data from a remote email server. |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#connection-parser_settings) | Initializes a new Parser to extract data from a remote email server. |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#file_path) | Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser/) class. |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#file_path-load_options) | Initializes a new Parser with the specified file path and load options. |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#file_path-parser_settings) | Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser/) class with [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings/). |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#file_path-load_options-parser_settings) | Initializes a new [`Parser`](/parser/python-net/groupdocs.parser/parser/) instance with the specified file path, optional load options, and parser settings. |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#document) | Initializes a new [`Parser`](/parser/python-net/groupdocs.parser/parser/) instance. |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#document-load_options) | Initializes a new Parser instance with the specified load options. |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#document-parser_settings) | Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser/) class with [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings/). |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#document-load_options-parser_settings) | Initializes a new Parser instance with the given document stream, load options, and parser settings. |

### Methods
| Method | Description |
| :- | :- |
| [dispose](/parser/python-net/groupdocs.parser/parser/dispose/) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [generate_adjustment_fields](/parser/python-net/groupdocs.parser/parser/generate_adjustment_fields/#options) | Generates fields for automatic adjustment of template position and scale. |
| [generate_adjustment_fields_adjustment_fields_options](/parser/python-net/groupdocs.parser/parser/generate_adjustment_fields_adjustment_fields_options/) |  |
| [generate_preview](/parser/python-net/groupdocs.parser/parser/generate_preview/#preview_options) | Generates pages preview. |
| [generate_preview_preview_options](/parser/python-net/groupdocs.parser/parser/generate_preview_preview_options/) |  |
| [get_annotations](/parser/python-net/groupdocs.parser/parser/get_annotations/) | Extracts annotations from the document. |
| [get_annotations](/parser/python-net/groupdocs.parser/parser/get_annotations/#page_index) | Extracts annotations from the document page. |
| [get_annotations_int32](/parser/python-net/groupdocs.parser/parser/get_annotations_int32/) |  |
| [get_barcodes](/parser/python-net/groupdocs.parser/parser/get_barcodes/) | Extracts barcodes from the document. |
| [get_barcodes](/parser/python-net/groupdocs.parser/parser/get_barcodes/#page_index) | Extracts barcodes from the document page. |
| [get_barcodes](/parser/python-net/groupdocs.parser/parser/get_barcodes/#options) | Extracts barcodes from the document using customization options (to set the rectangular area that contains barcodes). |
| [get_barcodes](/parser/python-net/groupdocs.parser/parser/get_barcodes/#options) | Extracts barcodes from the document using customization options. |
| [get_barcodes](/parser/python-net/groupdocs.parser/parser/get_barcodes/#page_index-options) | Extracts barcodes from a document page using customization options to set the rectangular area that contains barcodes. |
| [get_barcodes](/parser/python-net/groupdocs.parser/parser/get_barcodes/#page_index-options) | Extracts barcodes from the document page using customization options. |
| [get_barcodes_barcode_options](/parser/python-net/groupdocs.parser/parser/get_barcodes_barcode_options/) |  |
| [get_barcodes_int32](/parser/python-net/groupdocs.parser/parser/get_barcodes_int32/) |  |
| [get_barcodes_page_area_options](/parser/python-net/groupdocs.parser/parser/get_barcodes_page_area_options/) |  |
| [get_container](/parser/python-net/groupdocs.parser/parser/get_container/) | Extracts a container object from the document to work with formats that contain attachments, ZIP archives, etc. |
| [get_document_info](/parser/python-net/groupdocs.parser/parser/get_document_info/) | Returns the general information about the document. |
| [get_file_info](/parser/python-net/groupdocs.parser/parser/get_file_info/#file_path) | Returns the general information about a file. |
| [get_file_info](/parser/python-net/groupdocs.parser/parser/get_file_info/#file_path-load_options) | Returns the general information about a file. |
| [get_file_info](/parser/python-net/groupdocs.parser/parser/get_file_info/#document) | Returns the general information about a file. |
| [get_file_info](/parser/python-net/groupdocs.parser/parser/get_file_info/#document-load_options) | Returns the general information about a file. |
| [get_file_info_file](/parser/python-net/groupdocs.parser/parser/get_file_info_file/) |  |
| [get_file_info_stream](/parser/python-net/groupdocs.parser/parser/get_file_info_stream/) |  |
| [get_file_info_streams](/parser/python-net/groupdocs.parser/parser/get_file_info_streams/) |  |
| [get_file_info_string](/parser/python-net/groupdocs.parser/parser/get_file_info_string/) |  |
| [get_formatted_text](/parser/python-net/groupdocs.parser/parser/get_formatted_text/#options) | Extracts formatted text from the document. |
| [get_formatted_text](/parser/python-net/groupdocs.parser/parser/get_formatted_text/#page_index-options) | Extracts formatted text from a document page. |
| [get_formatted_text_formatted_text_options](/parser/python-net/groupdocs.parser/parser/get_formatted_text_formatted_text_options/) |  |
| [get_formatted_text_int32](/parser/python-net/groupdocs.parser/parser/get_formatted_text_int32/) |  |
| [get_highlight](/parser/python-net/groupdocs.parser/parser/get_highlight/#position-is_direct-options) | Extracts a highlight from the document. |
| [get_highlight_int32](/parser/python-net/groupdocs.parser/parser/get_highlight_int32/) |  |
| [get_hyperlinks](/parser/python-net/groupdocs.parser/parser/get_hyperlinks/) | Extracts hyperlinks from the document. |
| [get_hyperlinks](/parser/python-net/groupdocs.parser/parser/get_hyperlinks/#page_index) | Extracts hyperlinks from the document page. |
| [get_hyperlinks](/parser/python-net/groupdocs.parser/parser/get_hyperlinks/#options) | Extracts hyperlinks from the document using customization options (to set the rectangular area that contains hyperlinks). |
| [get_hyperlinks](/parser/python-net/groupdocs.parser/parser/get_hyperlinks/#page_index-options) | Extracts hyperlinks from the document page using customization options to set the rectangular area that contains hyperlinks. |
| [get_hyperlinks_int32](/parser/python-net/groupdocs.parser/parser/get_hyperlinks_int32/) |  |
| [get_hyperlinks_page_area_options](/parser/python-net/groupdocs.parser/parser/get_hyperlinks_page_area_options/) |  |
| [get_images](/parser/python-net/groupdocs.parser/parser/get_images/) | Extracts images from the document. |
| [get_images](/parser/python-net/groupdocs.parser/parser/get_images/#options) | Extracts images from the document using customization options (to set the rectangular area that contains images). |
| [get_images](/parser/python-net/groupdocs.parser/parser/get_images/#page_index) | Extracts images from the document page. |
| [get_images](/parser/python-net/groupdocs.parser/parser/get_images/#page_index-options) | Extracts images from the document page using customization options (to set the rectangular area that contains images). |
| [get_images_int32](/parser/python-net/groupdocs.parser/parser/get_images_int32/) |  |
| [get_images_page_area_options](/parser/python-net/groupdocs.parser/parser/get_images_page_area_options/) |  |
| [get_metadata](/parser/python-net/groupdocs.parser/parser/get_metadata/) | Extracts metadata from the document. |
| [get_page_preview](/parser/python-net/groupdocs.parser/parser/get_page_preview/#page_index) | Generates a document page preview. |
| [get_page_preview](/parser/python-net/groupdocs.parser/parser/get_page_preview/#page_index-options) | Generates a document page preview using customization options. |
| [get_page_preview_int32](/parser/python-net/groupdocs.parser/parser/get_page_preview_int32/) |  |
| [get_structure](/parser/python-net/groupdocs.parser/parser/get_structure/) | Extracts a structured text from the document. |
| [get_tables](/parser/python-net/groupdocs.parser/parser/get_tables/#options) | Extracts tables from the document. |
| [get_tables](/parser/python-net/groupdocs.parser/parser/get_tables/#page_index-options) | Extracts tables from the document page. |
| [get_tables](/parser/python-net/groupdocs.parser/parser/get_tables/) | Extracts tables from the document. |
| [get_tables](/parser/python-net/groupdocs.parser/parser/get_tables/#page_index) | Extracts tables from the document page. |
| [get_tables_int32](/parser/python-net/groupdocs.parser/parser/get_tables_int32/) |  |
| [get_tables_page_table_area_options](/parser/python-net/groupdocs.parser/parser/get_tables_page_table_area_options/) |  |
| [get_text](/parser/python-net/groupdocs.parser/parser/get_text/) | Extracts text from the document. |
| [get_text](/parser/python-net/groupdocs.parser/parser/get_text/#options) | Extracts a text page from the document using text options (to enable raw fast text extraction mode). |
| [get_text](/parser/python-net/groupdocs.parser/parser/get_text/#page_index) | Extracts text from a specific page of the document. |
| [get_text](/parser/python-net/groupdocs.parser/parser/get_text/#page_index-options) | Extracts text from a specific page of the document using text options (enables raw fast text extraction mode). |
| [get_text_areas](/parser/python-net/groupdocs.parser/parser/get_text_areas/) | Extracts text areas from the document. |
| [get_text_areas](/parser/python-net/groupdocs.parser/parser/get_text_areas/#options) | Extracts text areas from the document using customization options (regular expression, match case, etc.). |
| [get_text_areas](/parser/python-net/groupdocs.parser/parser/get_text_areas/#page_index) | Extracts text areas from the document page. |
| [get_text_areas](/parser/python-net/groupdocs.parser/parser/get_text_areas/#page_index-options) | Extracts text areas from the document page using customization options (regular expression, match case, etc.). |
| [get_text_areas_int32](/parser/python-net/groupdocs.parser/parser/get_text_areas_int32/) |  |
| [get_text_areas_page_text_area_options](/parser/python-net/groupdocs.parser/parser/get_text_areas_page_text_area_options/) |  |
| [get_text_int32](/parser/python-net/groupdocs.parser/parser/get_text_int32/) |  |
| [get_text_text_options](/parser/python-net/groupdocs.parser/parser/get_text_text_options/) |  |
| [get_toc](/parser/python-net/groupdocs.parser/parser/get_toc/) | Extracts a table of contents from the document. |
| [get_worksheet_cells](/parser/python-net/groupdocs.parser/parser/get_worksheet_cells/#worksheet_index) | Extracts worksheet cells. |
| [get_worksheet_cells](/parser/python-net/groupdocs.parser/parser/get_worksheet_cells/#worksheet_index-options) | Extracts worksheet cells using customization options. |
| [get_worksheet_cells_int32](/parser/python-net/groupdocs.parser/parser/get_worksheet_cells_int32/) |  |
| [get_worksheet_info](/parser/python-net/groupdocs.parser/parser/get_worksheet_info/) | Extracts the info about all worksheets in the spreadsheet. |
| [get_worksheet_info](/parser/python-net/groupdocs.parser/parser/get_worksheet_info/#worksheet_index) | Extracts the info about the worksheet. |
| [get_worksheet_info_int32](/parser/python-net/groupdocs.parser/parser/get_worksheet_info_int32/) |  |
| [parse_by_template](/parser/python-net/groupdocs.parser/parser/parse_by_template/#template) | Parses the document by the user-generated template. |
| [parse_by_template](/parser/python-net/groupdocs.parser/parser/parse_by_template/#template-options) | Parses the document by the user-generated template using customization options. |
| [parse_by_template](/parser/python-net/groupdocs.parser/parser/parse_by_template/#template_collection-options) | Selects the most suitable template from the provided collection and then parses the document against the selected template. |
| [parse_by_template_template](/parser/python-net/groupdocs.parser/parser/parse_by_template_template/) |  |
| [parse_by_template_template_collection](/parser/python-net/groupdocs.parser/parser/parse_by_template_template_collection/) |  |
| [parse_form](/parser/python-net/groupdocs.parser/parser/parse_form/) | Parses the document form. |
| [parse_pages_by_template](/parser/python-net/groupdocs.parser/parser/parse_pages_by_template/#template) | Parses the document pages using the user-generated template. |
| [parse_pages_by_template](/parser/python-net/groupdocs.parser/parser/parse_pages_by_template/#template-options) | Parses the document pages by the user-generated template using customization options. |
| [parse_pages_by_template_template](/parser/python-net/groupdocs.parser/parser/parse_pages_by_template_template/) |  |
| [search](/parser/python-net/groupdocs.parser/parser/search/#keyword) | Searches a keyword in the document. |
| [search](/parser/python-net/groupdocs.parser/parser/search/#keyword-options) | Searches a keyword in the document using search options (regular expression, match case, etc.). |
| [search_file](/parser/python-net/groupdocs.parser/parser/search_file/) |  |
| [search_string](/parser/python-net/groupdocs.parser/parser/search_string/) |  |

### Properties
| Property | Description |
| :- | :- |
| [features](/parser/python-net/groupdocs.parser/parser/features/) | The supported features. |

### Example

```python
from groupdocs.parser import Parser

with Parser("./sample.pdf") as parser:
    text_reader = parser.get_text()
    if text_reader is not None:
        print(text_reader.read_to_end())
```

### See Also
* module [`groupdocs.parser`](/parser/python-net/groupdocs.parser/)

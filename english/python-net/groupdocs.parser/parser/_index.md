---
title: Parser class
second_title: GroupDocs.Parser for Python via .NET API References
description: 
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
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#System.Uri) | Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class to extract data from an URI. |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#System.Uri-groupdocs.parser.options.LoadOptions) | Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class to extract data from an URI with `load_options`. |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#System.Uri-groupdocs.parser.options.ParserSettings) | Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class to extract data from an URI with `parser_settings`. |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#System.Uri-groupdocs.parser.options.LoadOptions-groupdocs.parser.options.ParserSettings) | Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class to extract data from an URI with `load_options` and `parser_settings`. |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#groupdocs.parser.options.EmailConnection) | Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class to extract data from a remote email server. |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#groupdocs.parser.options.EmailConnection-groupdocs.parser.options.ParserSettings) | Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class to extract data from a remote email server. |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#System.String) | Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class. |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#System.String-groupdocs.parser.options.LoadOptions) | Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class with [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions). |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#System.String-groupdocs.parser.options.ParserSettings) | Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class with [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings). |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#System.String-groupdocs.parser.options.LoadOptions-groupdocs.parser.options.ParserSettings) | Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class with [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions)<br/>and [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings). |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#io.RawIOBase) | Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class. |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#io.RawIOBase-groupdocs.parser.options.LoadOptions) | Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class with [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions). |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#io.RawIOBase-groupdocs.parser.options.ParserSettings) | Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class with [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings). |
| [__init__](/parser/python-net/groupdocs.parser/parser/__init__/#io.RawIOBase-groupdocs.parser.options.LoadOptions-groupdocs.parser.options.ParserSettings) | Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class with [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions)<br/>and [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings). |


### Properties
| Property | Description |
| :- | :- |
| [features](/parser/python-net/groupdocs.parser/parser/features) | Gets the supported features. |


### Methods
| Method | Description |
| :- | :- |
| [get_file_info](/parser/python-net/groupdocs.parser/parser/get_file_info/#System.String) | Returns the general information about a file. |
| [get_file_info](/parser/python-net/groupdocs.parser/parser/get_file_info/#System.String-groupdocs.parser.options.LoadOptions) | Returns the general information about a file. |
| [get_file_info](/parser/python-net/groupdocs.parser/parser/get_file_info/#io.RawIOBase) | Returns the general information about a file. |
| [get_file_info](/parser/python-net/groupdocs.parser/parser/get_file_info/#io.RawIOBase-groupdocs.parser.options.LoadOptions) | Returns the general information about a file. |
| [get_page_preview](/parser/python-net/groupdocs.parser/parser/get_page_preview/#int) | Generates a document page preview. |
| [get_page_preview](/parser/python-net/groupdocs.parser/parser/get_page_preview/#int-groupdocs.parser.options.PagePreviewOptions) | Generates a document page preview using customization options. |
| [get_text](/parser/python-net/groupdocs.parser/parser/get_text/#) | Extracts a text from the document. |
| [get_text](/parser/python-net/groupdocs.parser/parser/get_text/#groupdocs.parser.options.TextOptions) | Extracts a text page from the document using text options (to enable raw fast text extraction mode). |
| [get_text](/parser/python-net/groupdocs.parser/parser/get_text/#int) | Extracts a text from the document page. |
| [get_text](/parser/python-net/groupdocs.parser/parser/get_text/#int-groupdocs.parser.options.TextOptions) | Extracts a text from the document page using text options (to enable raw fast text extraction mode). |
| [get_formatted_text](/parser/python-net/groupdocs.parser/parser/get_formatted_text/#groupdocs.parser.options.FormattedTextOptions) | Extracts a formatted text from the document. |
| [get_formatted_text](/parser/python-net/groupdocs.parser/parser/get_formatted_text/#int-groupdocs.parser.options.FormattedTextOptions) | Extracts a formatted text from the document page. |
| [search](/parser/python-net/groupdocs.parser/parser/search/#System.String) | Searches a `keyword` in the document. |
| [search](/parser/python-net/groupdocs.parser/parser/search/#System.String-groupdocs.parser.options.SearchOptions) | Searches a `keyword` in the document using search options (regular expression, match case, etc.). |
| [get_text_areas](/parser/python-net/groupdocs.parser/parser/get_text_areas/#) | Extracts text areas from the document. |
| [get_text_areas](/parser/python-net/groupdocs.parser/parser/get_text_areas/#groupdocs.parser.options.PageTextAreaOptions) | Extracts text areas from the document using customization options (regular expression, match case, etc.). |
| [get_text_areas](/parser/python-net/groupdocs.parser/parser/get_text_areas/#int) | Extracts text areas from the document page. |
| [get_text_areas](/parser/python-net/groupdocs.parser/parser/get_text_areas/#int-groupdocs.parser.options.PageTextAreaOptions) | Extracts text areas from the document page using customization options (regular expression, match case, etc.). |
| [get_images](/parser/python-net/groupdocs.parser/parser/get_images/#) | Extracts images from the document. |
| [get_images](/parser/python-net/groupdocs.parser/parser/get_images/#groupdocs.parser.options.PageAreaOptions) | Extracts images from the document using customization options <br/>(to set the rectangular area that contains images). |
| [get_images](/parser/python-net/groupdocs.parser/parser/get_images/#int) | Extracts images from the document page. |
| [get_images](/parser/python-net/groupdocs.parser/parser/get_images/#int-groupdocs.parser.options.PageAreaOptions) | Extracts images from the document page using customization options <br/>(to set the rectangular area that contains images). |
| [get_hyperlinks](/parser/python-net/groupdocs.parser/parser/get_hyperlinks/#) | Extracts hyperlinks from the document. |
| [get_hyperlinks](/parser/python-net/groupdocs.parser/parser/get_hyperlinks/#int) | Extracts hyperlinks from the document page. |
| [get_hyperlinks](/parser/python-net/groupdocs.parser/parser/get_hyperlinks/#groupdocs.parser.options.PageAreaOptions) | Extracts hyperlinks from the document using customization options <br/>(to set the rectangular area that contains hyperlinks). |
| [get_hyperlinks](/parser/python-net/groupdocs.parser/parser/get_hyperlinks/#int-groupdocs.parser.options.PageAreaOptions) | Extracts hyperlinks from the document page using customization options <br/>(to set the rectangular area that contains hyperlinks). |
| [get_barcodes](/parser/python-net/groupdocs.parser/parser/get_barcodes/#) | Extracts barcodes from the document. |
| [get_barcodes](/parser/python-net/groupdocs.parser/parser/get_barcodes/#int) | Extracts barcodes from the document page. |
| [get_barcodes](/parser/python-net/groupdocs.parser/parser/get_barcodes/#groupdocs.parser.options.PageAreaOptions) | Extracts barcodes from the document using customization options <br/>(to set the rectangular area that contains barcodes). |
| [get_barcodes](/parser/python-net/groupdocs.parser/parser/get_barcodes/#groupdocs.parser.options.BarcodeOptions) | Extracts barcodes from the document using customization options. |
| [get_barcodes](/parser/python-net/groupdocs.parser/parser/get_barcodes/#int-groupdocs.parser.options.PageAreaOptions) | Extracts barcodes from the document page using customization options <br/>(to set the rectangular area that contains barcodes). |
| [get_barcodes](/parser/python-net/groupdocs.parser/parser/get_barcodes/#int-groupdocs.parser.options.BarcodeOptions) | Extracts barcodes from the document page using customization options. |
| [get_tables](/parser/python-net/groupdocs.parser/parser/get_tables/#groupdocs.parser.options.PageTableAreaOptions) | Extracts tables from the document. |
| [get_tables](/parser/python-net/groupdocs.parser/parser/get_tables/#int-groupdocs.parser.options.PageTableAreaOptions) | Extracts tables from the document page. |
| [get_tables](/parser/python-net/groupdocs.parser/parser/get_tables/#) | Extracts tables from the document. |
| [get_tables](/parser/python-net/groupdocs.parser/parser/get_tables/#int) | Extracts tables from the document page. |
| [get_worksheet_info](/parser/python-net/groupdocs.parser/parser/get_worksheet_info/#) | Extracts the info about all worksheets in the spreadsheet. |
| [get_worksheet_info](/parser/python-net/groupdocs.parser/parser/get_worksheet_info/#int) | Extracts the info about the worksheet. |
| [get_worksheet_cells](/parser/python-net/groupdocs.parser/parser/get_worksheet_cells/#int) | Extracts worksheet cells. |
| [get_worksheet_cells](/parser/python-net/groupdocs.parser/parser/get_worksheet_cells/#int-groupdocs.parser.options.WorksheetOptions) | Extracts worksheet cells using customization options. |
| [parse_by_template](/parser/python-net/groupdocs.parser/parser/parse_by_template/#groupdocs.parser.templates.Template) | Parses the document by the user-generated template. |
| [parse_by_template](/parser/python-net/groupdocs.parser/parser/parse_by_template/#groupdocs.parser.templates.Template-groupdocs.parser.options.ParseByTemplateOptions) | Parses the document by the user-generated template using customization options. |
| [parse_by_template](/parser/python-net/groupdocs.parser/parser/parse_by_template/#groupdocs.parser.templates.TemplateCollection-groupdocs.parser.options.ParseByTemplateOptions) | Selects the most suitable template from the provided collection and then parses the document against the selected template. |
| [parse_pages_by_template](/parser/python-net/groupdocs.parser/parser/parse_pages_by_template/#groupdocs.parser.templates.Template) | Parses the document pages by the user-generated template. |
| [parse_pages_by_template](/parser/python-net/groupdocs.parser/parser/parse_pages_by_template/#groupdocs.parser.templates.Template-groupdocs.parser.options.ParseByTemplateOptions) | Parses the document pages by the user-generated template using customization options. |
| [generate_preview](/parser/python-net/groupdocs.parser/parser/generate_preview/#groupdocs.parser.options.PreviewOptions) | Get pages preview. |
| [get_document_info](/parser/python-net/groupdocs.parser/parser/get_document_info/#) | Returns the general information about the document. |
| [get_highlight](/parser/python-net/groupdocs.parser/parser/get_highlight/#int-bool-groupdocs.parser.options.HighlightOptions) | Extracts a highlight from the document. |
| [get_toc](/parser/python-net/groupdocs.parser/parser/get_toc/#) | Extracts a table of contents from the document. |
| [get_container](/parser/python-net/groupdocs.parser/parser/get_container/#) | Extracts a container object from the document to work with formats that contain attachments, ZIP archives etc. |
| [get_metadata](/parser/python-net/groupdocs.parser/parser/get_metadata/#) | Extracts metadata from the document. |
| [generate_adjustment_fields](/parser/python-net/groupdocs.parser/parser/generate_adjustment_fields/#groupdocs.parser.options.AdjustmentFieldsOptions) | Generates fields for automatic adjustment of template position and scale. |
| [parse_form](/parser/python-net/groupdocs.parser/parser/parse_form/#) | Parses the document form. |



### See Also
* module [`groupdocs.parser`](..)
* class [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions)
* class [`Parser`](/parser/python-net/groupdocs.parser/parser)
* class [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings)

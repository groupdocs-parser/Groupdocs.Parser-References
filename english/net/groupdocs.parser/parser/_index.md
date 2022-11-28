---
title: Parser
second_title: GroupDocs.Parser for .NET API Reference
description: Represents the main class that controls text images container extraction and parsing functionality.
type: docs
weight: 620
url: /net/groupdocs.parser/parser/
---
## Parser class

Represents the main class that controls text, images, container extraction and parsing functionality.

```csharp
public sealed class Parser : IDisposable
```

## Constructors

| Name | Description |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | Initializes a new instance of the [`Parser`](../parser) class to extract data from a database. |
| [Parser](parser#constructor)(EmailConnection) | Initializes a new instance of the [`Parser`](../parser) class to extract data from a remote email server. |
| [Parser](parser#constructor_4)(Stream) | Initializes a new instance of the [`Parser`](../parser) class. |
| [Parser](parser#constructor_8)(string) | Initializes a new instance of the [`Parser`](../parser) class. |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | Initializes a new instance of the [`Parser`](../parser) class to extract data from a database. |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | Initializes a new instance of the [`Parser`](../parser) class to extract data from a remote email server. |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | Initializes a new instance of the [`Parser`](../parser) class with [`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [Parser](parser#constructor_7)(Stream, ParserSettings) | Initializes a new instance of the [`Parser`](../parser) class with [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_9)(string, LoadOptions) | Initializes a new instance of the [`Parser`](../parser) class with [`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [Parser](parser#constructor_11)(string, ParserSettings) | Initializes a new instance of the [`Parser`](../parser) class with [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | Initializes a new instance of the [`Parser`](../parser) class with [`LoadOptions`](../../groupdocs.parser.options/loadoptions) and [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_10)(string, LoadOptions, ParserSettings) | Initializes a new instance of the [`Parser`](../parser) class with [`LoadOptions`](../../groupdocs.parser.options/loadoptions) and [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |

## Properties

| Name | Description |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | Gets the supported features. |

## Methods

| Name | Description |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | Get pages preview. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | Extracts barcodes from the document. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_2)(int) | Extracts barcodes from the document page. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(PageAreaOptions) | Extracts barcodes from the document using customization options (to set the rectangular area that contains barcodes). |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int, PageAreaOptions) | Extracts barcodes from the document page using customization options (to set the rectangular area that contains barcodes). |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | Extracts a container object from the document to work with formats that contain attachments, ZIP archives etc. |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | Returns the general information about the document. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | Extracts a formatted text from the document. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | Extracts a formatted text from the document page. |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | Extracts a highlight from the document. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | Extracts hyperlinks from the document. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | Extracts hyperlinks from the document page. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | Extracts hyperlinks from the document using customization options (to set the rectangular area that contains hyperlinks). |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | Extracts hyperlinks from the document page using customization options (to set the rectangular area that contains hyperlinks). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | Extracts images from the document. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | Extracts images from the document page. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | Extracts images from the document using customization options (to set the rectangular area that contains images). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | Extracts images from the document page using customization options (to set the rectangular area that contains images). |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | Extracts metadata from the document. |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | Extracts a structured text from the document. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)(PageTableAreaOptions) | Extracts tables from the document. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(int, PageTableAreaOptions) | Extracts tables from the document page. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | Extracts a text from the document. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | Extracts a text from the document page. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | Extracts a text page from the document using text options (to enable raw fast text extraction mode). |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | Extracts a text from the document page using text options (to enable raw fast text extraction mode). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | Extracts text areas from the document. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | Extracts text areas from the document page. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | Extracts text areas from the document using customization options (regular expression, match case, etc.). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | Extracts text areas from the document page using customization options (regular expression, match case, etc.). |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | Extracts a table of contents from the document. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate)(Template) | Parses the document by the user-generated template. |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | Parses the document form. |
| [Search](../../groupdocs.parser/parser/search#search)(string) | Searches a *keyword* in the document. |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | Searches a *keyword* in the document using search options (regular expression, match case, etc.). |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | Returns the general information about a file. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | Returns the general information about a file. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | Returns the general information about a file. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | Returns the general information about a file. |

### See Also

* namespace [GroupDocs.Parser](../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.parser.dll -->

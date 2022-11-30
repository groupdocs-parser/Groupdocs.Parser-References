---
title: com.groupdocs.parser.options
second_title: GroupDocs.Parser for Java API Reference
description: The package provides classes to specify additional options when parsing data from documents.
type: docs
weight: 14
url: /java/com.groupdocs.parser.options/
---

The package provides classes to specify additional options when parsing data from documents.


## Classes

| Class | Description |
| --- | --- |
| [DocumentInfo](../com.groupdocs.parser.options/documentinfo) | Represents the document information. |
| [EmailConnection](../com.groupdocs.parser.options/emailconnection) | Represents the email connection information. |
| [EmailEwsConnection](../com.groupdocs.parser.options/emailewsconnection) | Represents the email connection information for EWS protocol. |
| [EmailImapConnection](../com.groupdocs.parser.options/emailimapconnection) | Represents the email connection information for IMAP protocol. |
| [EmailPopConnection](../com.groupdocs.parser.options/emailpopconnection) | Represents the email connection information for POP protocol. |
| [Features](../com.groupdocs.parser.options/features) | Represents the supported features list. |
| [FileInfo](../com.groupdocs.parser.options/fileinfo) | Represents the file information. |
| [FileType](../com.groupdocs.parser.options/filetype) | Represents the file type. |
| [FormattedTextOptions](../com.groupdocs.parser.options/formattedtextoptions) | Provides the options which are used for formatted text extraction. |
| [HighlightOptions](../com.groupdocs.parser.options/highlightoptions) | Provides the options which are used to extract a highlight (a block of text aroud found text in search scenarios). |
| [ImageOptions](../com.groupdocs.parser.options/imageoptions) | Provides the options which are used for image extraction. |
| [LoadOptions](../com.groupdocs.parser.options/loadoptions) | Provides the options which are used to open a file. |
| [OcrConnectorBase](../com.groupdocs.parser.options/ocrconnectorbase) | Provides the OCR functionality. |
| [OcrEventHandler](../com.groupdocs.parser.options/ocreventhandler) | Provides a handler for OCR events. |
| [OcrOptions](../com.groupdocs.parser.options/ocroptions) | Provides the options which are used for OCR Connector. |
| [PageAreaOptions](../com.groupdocs.parser.options/pageareaoptions) | Provides the options which are used for page areas extraction. |
| [PageInfo](../com.groupdocs.parser.options/pageinfo) | Represents the document page information. |
| [PageRenderInfo](../com.groupdocs.parser.options/pagerenderinfo) | Represents the information of how a page is rendered. |
| [PageTableAreaOptions](../com.groupdocs.parser.options/pagetableareaoptions) | Provides the options which are used for page table areas extraction. |
| [PageTextAreaOptions](../com.groupdocs.parser.options/pagetextareaoptions) | Provides the options which are used for page text areas extraction. |
| [ParserSettings](../com.groupdocs.parser.options/parsersettings) | Provides the settings which are used to customize data extraction. |
| [PreviewOptions](../com.groupdocs.parser.options/previewoptions) | Provides options to sets requirements and stream delegates for preview generation. |
| [SearchOptions](../com.groupdocs.parser.options/searchoptions) | Provides the options which are used for text search. |
| [TextDocumentInfo](../com.groupdocs.parser.options/textdocumentinfo) | Represents the text document information. |
| [TextOptions](../com.groupdocs.parser.options/textoptions) | Provides the options which are used for text extraction. |

## Interfaces

| Interface | Description |
| --- | --- |
| [ICreatePageStream](../com.groupdocs.parser.options/icreatepagestream) | Represents a delegate that returns a stream to write page preview data. |
| [IDocumentInfo](../com.groupdocs.parser.options/idocumentinfo) | Represents the document information. |
| [ILogger](../com.groupdocs.parser.options/ilogger) | Defines the interface of a logger that is used for logging events and errors during data extraction. |
| [IPreviewPageRender](../com.groupdocs.parser.options/ipreviewpagerender) | Represents a method which is called before a document page is rendered. |
| [IReleasePageStream](../com.groupdocs.parser.options/ireleasepagestream) | Represents a method which releases the stream created by the [ICreatePageStream](../com.groupdocs.parser.options/icreatepagestream) delegate. |

## Enumerations

| Enum | Description |
| --- | --- |
| [FileFormat](../com.groupdocs.parser.options/fileformat) | Defines a type of the file. |
| [FileTypeDetectionMode](../com.groupdocs.parser.options/filetypedetectionmode) | Defines a mode of the file type detection. |
| [FormattedTextMode](../com.groupdocs.parser.options/formattedtextmode) | Defines a formatted text mode. |
| [ImageFormat](../com.groupdocs.parser.options/imageformat) | Defines a format of the image. |
| [PreviewFormats](../com.groupdocs.parser.options/previewformats) | Represents supported preview formats. |

---
title: "com.groupdocs.parser.options"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Paketet tillhandahåller klasser för att specificera ytterligare alternativ när data parsas från dokument."
type: docs
weight: 15
url: /sv/java/com.groupdocs.parser.options/
---

Paketet tillhandahåller klasser för att specificera ytterligare alternativ när data parsas från dokument.



## Klasser

| Klass | Beskrivning |
| --- | --- |
| [BarcodeOptions](../com.groupdocs.parser.options/barcodeoptions) | Tillhandahåller de alternativ som används för streckkodsextraktion. |
| [DocumentInfo](../com.groupdocs.parser.options/documentinfo) | Representerar dokumentinformationen. |
| [EmailConnection](../com.groupdocs.parser.options/emailconnection) | Representerar e-postanslutningsinformationen. |
| [EmailEwsConnection](../com.groupdocs.parser.options/emailewsconnection) | Representerar e-postanslutningsinformationen för EWS-protokollet. |
| [EmailImapConnection](../com.groupdocs.parser.options/emailimapconnection) | Representerar e-postanslutningsinformationen för IMAP-protokollet. |
| [EmailPopConnection](../com.groupdocs.parser.options/emailpopconnection) | Representerar e-postanslutningsinformationen för POP-protokollet. |
| [ExternalResourceHandler](../com.groupdocs.parser.options/externalresourcehandler) | Tillhandahåller en hanterare för inläsning av externa resurser. |
| [ExternalResourceLoadingArgs](../com.groupdocs.parser.options/externalresourceloadingargs) | Tillhandahåller data för metoden [ExternalResourceHandler.#onLoading(ExternalResourceLoadingArgs)](../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-). |
| [Features](../com.groupdocs.parser.options/features) | Representerar listan över stödda funktioner. |
| [FileInfo](../com.groupdocs.parser.options/fileinfo) | Representerar filinformationen. |
| [FileType](../com.groupdocs.parser.options/filetype) | Representerar filtypen. |
| [FormattedTextOptions](../com.groupdocs.parser.options/formattedtextoptions) | Tillhandahåller de alternativ som används för formaterad textutvinning. |
| [HighlightOptions](../com.groupdocs.parser.options/highlightoptions) | Tillhandahåller de alternativ som används för att extrahera en markering (ett textblock runt hittad text i sökscenarier). |
| [ImageOptions](../com.groupdocs.parser.options/imageoptions) | Tillhandahåller de alternativ som används för bildutvinning. |
| [LoadOptions](../com.groupdocs.parser.options/loadoptions) | Tillhandahåller de alternativ som används för att öppna en fil. |
| [OcrConnectorBase](../com.groupdocs.parser.options/ocrconnectorbase) | Tillhandahåller OCR-funktionaliteten. |
| [OcrEventHandler](../com.groupdocs.parser.options/ocreventhandler) | Tillhandahåller en hanterare för OCR-händelser. |
| [OcrOptions](../com.groupdocs.parser.options/ocroptions) | Tillhandahåller de alternativ som används för OCR-Connector. |
| [PageAreaOptions](../com.groupdocs.parser.options/pageareaoptions) | Tillhandahåller de alternativ som används för extrahering av sidområden. |
| [PageInfo](../com.groupdocs.parser.options/pageinfo) | Representerar informationen om dokumentets sida. |
| [PageRenderInfo](../com.groupdocs.parser.options/pagerenderinfo) | Representerar information om hur en sida renderas. |
| [PageTableAreaOptions](../com.groupdocs.parser.options/pagetableareaoptions) | Tillhandahåller de alternativ som används för extrahering av sidtabellområden. |
| [PageTextAreaOptions](../com.groupdocs.parser.options/pagetextareaoptions) | Tillhandahåller de alternativ som används för extrahering av sidtextområden. |
| [ParserSettings](../com.groupdocs.parser.options/parsersettings) | Tillhandahåller inställningarna som används för att anpassa datautvinning. |
| [PreviewOptions](../com.groupdocs.parser.options/previewoptions) | Tillhandahåller alternativ för att ange krav och strömdelegater för förhandsgranskningsgenerering. |
| [SearchOptions](../com.groupdocs.parser.options/searchoptions) | Tillhandahåller de alternativ som används för textsökning. |
| [TextDocumentInfo](../com.groupdocs.parser.options/textdocumentinfo) | Representerar informationen om textdokumentet. |
| [TextOptions](../com.groupdocs.parser.options/textoptions) | Tillhandahåller de alternativ som används för textutvinning. |

## Gränssnitt

| Gränssnitt | Beskrivning |
| --- | --- |
| [ICreatePageStream](../com.groupdocs.parser.options/icreatepagestream) | Representerar en delegat som returnerar en ström för att skriva förhandsgranskningsdata för sidan. |
| [IDocumentInfo](../com.groupdocs.parser.options/idocumentinfo) | Representerar dokumentinformationen. |
| [ILogger](../com.groupdocs.parser.options/ilogger) | Definierar gränssnittet för en logger som används för att logga händelser och fel under dataextraktion. |
| [IPreviewPageRender](../com.groupdocs.parser.options/ipreviewpagerender) | Representerar en metod som anropas innan en dokumentsida renderas. |
| [IReleasePageStream](../com.groupdocs.parser.options/ireleasepagestream) | Representerar en metod som frigör strömmen som skapats av delegaten [ICreatePageStream](../com.groupdocs.parser.options/icreatepagestream). |

## Enumerationer

| Enum | Beskrivning |
| --- | --- |
| [FileFormat](../com.groupdocs.parser.options/fileformat) | Definierar en typ av fil. |
| [FileTypeDetectionMode](../com.groupdocs.parser.options/filetypedetectionmode) | Definierar ett läge för filtypdetektering. |
| [FormattedTextMode](../com.groupdocs.parser.options/formattedtextmode) | Definierar ett formaterat textläge. |
| [ImageFormat](../com.groupdocs.parser.options/imageformat) | Definierar ett format för bilden. |
| [PreviewFormats](../com.groupdocs.parser.options/previewformats) | Representerar stödda förhandsgranskningsformat. |
| [QualityMode](../com.groupdocs.parser.options/qualitymode) | Definierar en kvalitetsnivå. |

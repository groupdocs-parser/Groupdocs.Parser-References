---
title: "com.groupdocs.parser.options"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Das Paket stellt Klassen bereit, um zusätzliche Optionen beim Parsen von Daten aus Dokumenten anzugeben."
type: docs
weight: 15
url: /de/java/com.groupdocs.parser.options/
---

Das Paket stellt Klassen bereit, um zusätzliche Optionen beim Parsen von Daten aus Dokumenten anzugeben.



## Klassen

| Klasse | Beschreibung |
| --- | --- |
| [BarcodeOptions](../com.groupdocs.parser.options/barcodeoptions) | Stellt die Optionen bereit, die für die Barcode‑Extraktion verwendet werden. |
| [DocumentInfo](../com.groupdocs.parser.options/documentinfo) | Stellt die Dokumentinformationen dar. |
| [EmailConnection](../com.groupdocs.parser.options/emailconnection) | Stellt die E‑Mail‑Verbindungsinformationen dar. |
| [EmailEwsConnection](../com.groupdocs.parser.options/emailewsconnection) | Stellt die E‑Mail‑Verbindungsinformationen für das EWS‑Protokoll dar. |
| [EmailImapConnection](../com.groupdocs.parser.options/emailimapconnection) | Stellt die E‑Mail‑Verbindungsinformationen für das IMAP‑Protokoll dar. |
| [EmailPopConnection](../com.groupdocs.parser.options/emailpopconnection) | Stellt die E‑Mail‑Verbindungsinformationen für das POP‑Protokoll dar. |
| [ExternalResourceHandler](../com.groupdocs.parser.options/externalresourcehandler) | Stellt einen Handler für das Laden externer Ressourcen bereit. |
| [ExternalResourceLoadingArgs](../com.groupdocs.parser.options/externalresourceloadingargs) | Stellt die Daten für die Methode [ExternalResourceHandler.#onLoading(ExternalResourceLoadingArgs)](../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-) bereit. |
| [Features](../com.groupdocs.parser.options/features) | Stellt die Liste der unterstützten Funktionen dar. |
| [FileInfo](../com.groupdocs.parser.options/fileinfo) | Stellt die Dateiinformationen dar. |
| [FileType](../com.groupdocs.parser.options/filetype) | Stellt den Dateityp dar. |
| [FormattedTextOptions](../com.groupdocs.parser.options/formattedtextoptions) | Stellt die Optionen bereit, die für die Extraktion formatierten Textes verwendet werden. |
| [HighlightOptions](../com.groupdocs.parser.options/highlightoptions) | Stellt die Optionen bereit, die zum Extrahieren einer Hervorhebung (eines Textblocks um gefundenen Text in Suchszenarien) verwendet werden. |
| [ImageOptions](../com.groupdocs.parser.options/imageoptions) | Stellt die Optionen bereit, die für die Bildextraktion verwendet werden. |
| [LoadOptions](../com.groupdocs.parser.options/loadoptions) | Stellt die Optionen bereit, die zum Öffnen einer Datei verwendet werden. |
| [OcrConnectorBase](../com.groupdocs.parser.options/ocrconnectorbase) | Stellt die OCR-Funktionalität bereit. |
| [OcrEventHandler](../com.groupdocs.parser.options/ocreventhandler) | Stellt einen Handler für OCR-Ereignisse bereit. |
| [OcrOptions](../com.groupdocs.parser.options/ocroptions) | Stellt die Optionen bereit, die für den OCR-Connector verwendet werden. |
| [PageAreaOptions](../com.groupdocs.parser.options/pageareaoptions) | Stellt die Optionen bereit, die für die Extraktion von Seitenbereichen verwendet werden. |
| [PageInfo](../com.groupdocs.parser.options/pageinfo) | Stellt die Informationen zur Dokumentenseite dar. |
| [PageRenderInfo](../com.groupdocs.parser.options/pagerenderinfo) | Stellt die Informationen darüber dar, wie eine Seite gerendert wird. |
| [PageTableAreaOptions](../com.groupdocs.parser.options/pagetableareaoptions) | Stellt die Optionen bereit, die für die Extraktion von Tabellenseitenbereichen verwendet werden. |
| [PageTextAreaOptions](../com.groupdocs.parser.options/pagetextareaoptions) | Stellt die Optionen bereit, die für die Extraktion von Textbereichen einer Seite verwendet werden. |
| [ParserSettings](../com.groupdocs.parser.options/parsersettings) | Stellt die Einstellungen bereit, die zur Anpassung der Datenerfassung verwendet werden. |
| [PreviewOptions](../com.groupdocs.parser.options/previewoptions) | Stellt Optionen bereit, um Anforderungen und Stream-Delegaten für die Vorschauerstellung festzulegen. |
| [SearchOptions](../com.groupdocs.parser.options/searchoptions) | Stellt die Optionen bereit, die für die Textsuche verwendet werden. |
| [TextDocumentInfo](../com.groupdocs.parser.options/textdocumentinfo) | Stellt die Informationen zum Textdokument dar. |
| [TextOptions](../com.groupdocs.parser.options/textoptions) | Stellt die Optionen bereit, die für die Textextraktion verwendet werden. |

## Schnittstellen

| Schnittstelle | Beschreibung |
| --- | --- |
| [ICreatePageStream](../com.groupdocs.parser.options/icreatepagestream) | Stellt einen Delegaten dar, der einen Stream zurückgibt, um Seitenvorschau-Daten zu schreiben. |
| [IDocumentInfo](../com.groupdocs.parser.options/idocumentinfo) | Stellt die Dokumentinformationen dar. |
| [ILogger](../com.groupdocs.parser.options/ilogger) | Definiert die Schnittstelle eines Loggers, der zum Protokollieren von Ereignissen und Fehlern während der Datenextraktion verwendet wird. |
| [IPreviewPageRender](../com.groupdocs.parser.options/ipreviewpagerender) | Stellt eine Methode dar, die aufgerufen wird, bevor eine Dokumentenseite gerendert wird. |
| [IReleasePageStream](../com.groupdocs.parser.options/ireleasepagestream) | Stellt eine Methode dar, die den von dem [ICreatePageStream](../com.groupdocs.parser.options/icreatepagestream)-Delegaten erstellten Stream freigibt. |

## Aufzählungen

| Enum | Beschreibung |
| --- | --- |
| [FileFormat](../com.groupdocs.parser.options/fileformat) | Definiert einen Dateityp. |
| [FileTypeDetectionMode](../com.groupdocs.parser.options/filetypedetectionmode) | Definiert einen Modus der Dateityp-Erkennung. |
| [FormattedTextMode](../com.groupdocs.parser.options/formattedtextmode) | Definiert einen formatierten Textmodus. |
| [ImageFormat](../com.groupdocs.parser.options/imageformat) | Definiert ein Bildformat. |
| [PreviewFormats](../com.groupdocs.parser.options/previewformats) | Stellt unterstützte Vorschaueformate dar. |
| [QualityMode](../com.groupdocs.parser.options/qualitymode) | Definiert ein Qualitätsniveau. |

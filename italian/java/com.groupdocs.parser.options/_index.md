---
title: "com.groupdocs.parser.options"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Il pacchetto fornisce classi per specificare opzioni aggiuntive durante l'analisi dei dati dai documenti."
type: docs
weight: 15
url: /it/java/com.groupdocs.parser.options/
---

Il pacchetto fornisce classi per specificare opzioni aggiuntive durante l'analisi dei dati dai documenti.



## Classi

| Classe | Descrizione |
| --- | --- |
| [BarcodeOptions](../com.groupdocs.parser.options/barcodeoptions) | Fornisce le opzioni utilizzate per l'estrazione dei codici a barre. |
| [DocumentInfo](../com.groupdocs.parser.options/documentinfo) | Rappresenta le informazioni del documento. |
| [EmailConnection](../com.groupdocs.parser.options/emailconnection) | Rappresenta le informazioni di connessione email. |
| [EmailEwsConnection](../com.groupdocs.parser.options/emailewsconnection) | Rappresenta le informazioni di connessione email per il protocollo EWS. |
| [EmailImapConnection](../com.groupdocs.parser.options/emailimapconnection) | Rappresenta le informazioni di connessione email per il protocollo IMAP. |
| [EmailPopConnection](../com.groupdocs.parser.options/emailpopconnection) | Rappresenta le informazioni di connessione email per il protocollo POP. |
| [ExternalResourceHandler](../com.groupdocs.parser.options/externalresourcehandler) | Fornisce un gestore per il caricamento di risorse esterne. |
| [ExternalResourceLoadingArgs](../com.groupdocs.parser.options/externalresourceloadingargs) | Fornisce i dati per il metodo [ExternalResourceHandler.#onLoading(ExternalResourceLoadingArgs)](../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-). |
| [Features](../com.groupdocs.parser.options/features) | Rappresenta l'elenco delle funzionalità supportate. |
| [FileInfo](../com.groupdocs.parser.options/fileinfo) | Rappresenta le informazioni del file. |
| [FileType](../com.groupdocs.parser.options/filetype) | Rappresenta il tipo di file. |
| [FormattedTextOptions](../com.groupdocs.parser.options/formattedtextoptions) | Fornisce le opzioni utilizzate per l'estrazione di testo formattato. |
| [HighlightOptions](../com.groupdocs.parser.options/highlightoptions) | Fornisce le opzioni utilizzate per estrarre un'evidenziazione (un blocco di testo intorno al testo trovato in scenari di ricerca). |
| [ImageOptions](../com.groupdocs.parser.options/imageoptions) | Fornisce le opzioni utilizzate per l'estrazione di immagini. |
| [LoadOptions](../com.groupdocs.parser.options/loadoptions) | Fornisce le opzioni utilizzate per aprire un file. |
| [OcrConnectorBase](../com.groupdocs.parser.options/ocrconnectorbase) | Fornisce la funzionalità OCR. |
| [OcrEventHandler](../com.groupdocs.parser.options/ocreventhandler) | Fornisce un gestore per gli eventi OCR. |
| [OcrOptions](../com.groupdocs.parser.options/ocroptions) | Fornisce le opzioni utilizzate per il connettore OCR. |
| [PageAreaOptions](../com.groupdocs.parser.options/pageareaoptions) | Fornisce le opzioni utilizzate per l'estrazione delle aree di pagina. |
| [PageInfo](../com.groupdocs.parser.options/pageinfo) | Rappresenta le informazioni della pagina del documento. |
| [PageRenderInfo](../com.groupdocs.parser.options/pagerenderinfo) | Rappresenta le informazioni su come una pagina viene renderizzata. |
| [PageTableAreaOptions](../com.groupdocs.parser.options/pagetableareaoptions) | Fornisce le opzioni utilizzate per l'estrazione delle aree di tabella della pagina. |
| [PageTextAreaOptions](../com.groupdocs.parser.options/pagetextareaoptions) | Fornisce le opzioni utilizzate per l'estrazione delle aree di testo della pagina. |
| [ParserSettings](../com.groupdocs.parser.options/parsersettings) | Fornisce le impostazioni utilizzate per personalizzare l'estrazione dei dati. |
| [PreviewOptions](../com.groupdocs.parser.options/previewoptions) | Fornisce opzioni per impostare i requisiti e i delegati di stream per la generazione dell'anteprima. |
| [SearchOptions](../com.groupdocs.parser.options/searchoptions) | Fornisce le opzioni utilizzate per la ricerca di testo. |
| [TextDocumentInfo](../com.groupdocs.parser.options/textdocumentinfo) | Rappresenta le informazioni del documento di testo. |
| [TextOptions](../com.groupdocs.parser.options/textoptions) | Fornisce le opzioni utilizzate per l'estrazione di testo. |

## Interfacce

| Interfaccia | Descrizione |
| --- | --- |
| [ICreatePageStream](../com.groupdocs.parser.options/icreatepagestream) | Rappresenta un delegato che restituisce uno stream per scrivere i dati dell'anteprima della pagina. |
| [IDocumentInfo](../com.groupdocs.parser.options/idocumentinfo) | Rappresenta le informazioni del documento. |
| [ILogger](../com.groupdocs.parser.options/ilogger) | Definisce l'interfaccia di un logger utilizzato per registrare eventi ed errori durante l'estrazione dei dati. |
| [IPreviewPageRender](../com.groupdocs.parser.options/ipreviewpagerender) | Rappresenta un metodo che viene chiamato prima che una pagina del documento venga renderizzata. |
| [IReleasePageStream](../com.groupdocs.parser.options/ireleasepagestream) | Rappresenta un metodo che rilascia lo stream creato dal delegato [ICreatePageStream](../com.groupdocs.parser.options/icreatepagestream). |

## Enumerazioni

| Enum | Descrizione |
| --- | --- |
| [FileFormat](../com.groupdocs.parser.options/fileformat) | Definisce un tipo di file. |
| [FileTypeDetectionMode](../com.groupdocs.parser.options/filetypedetectionmode) | Definisce una modalità di rilevamento del tipo di file. |
| [FormattedTextMode](../com.groupdocs.parser.options/formattedtextmode) | Definisce una modalità di testo formattato. |
| [ImageFormat](../com.groupdocs.parser.options/imageformat) | Definisce un formato dell'immagine. |
| [PreviewFormats](../com.groupdocs.parser.options/previewformats) | Rappresenta i formati di anteprima supportati. |
| [QualityMode](../com.groupdocs.parser.options/qualitymode) | Definisce un livello di qualità. |

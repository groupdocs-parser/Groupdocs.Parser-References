---
title: "com.groupdocs.parser.options"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "El paquete proporciona clases para especificar opciones adicionales al analizar datos de documentos."
type: docs
weight: 15
url: /es/java/com.groupdocs.parser.options/
---

El paquete proporciona clases para especificar opciones adicionales al analizar datos de documentos.



## Clases

| Clase | Descripción |
| --- | --- |
| [BarcodeOptions](../com.groupdocs.parser.options/barcodeoptions) | Proporciona las opciones que se utilizan para la extracción de códigos de barras. |
| [DocumentInfo](../com.groupdocs.parser.options/documentinfo) | Representa la información del documento. |
| [EmailConnection](../com.groupdocs.parser.options/emailconnection) | Representa la información de conexión del correo electrónico. |
| [EmailEwsConnection](../com.groupdocs.parser.options/emailewsconnection) | Representa la información de conexión del correo electrónico para el protocolo EWS. |
| [EmailImapConnection](../com.groupdocs.parser.options/emailimapconnection) | Representa la información de conexión del correo electrónico para el protocolo IMAP. |
| [EmailPopConnection](../com.groupdocs.parser.options/emailpopconnection) | Representa la información de conexión del correo electrónico para el protocolo POP. |
| [ExternalResourceHandler](../com.groupdocs.parser.options/externalresourcehandler) | Proporciona un controlador para la carga de recursos externos. |
| [ExternalResourceLoadingArgs](../com.groupdocs.parser.options/externalresourceloadingargs) | Proporciona los datos para el método [ExternalResourceHandler.#onLoading(ExternalResourceLoadingArgs)](../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-). |
| [Features](../com.groupdocs.parser.options/features) | Representa la lista de funciones compatibles. |
| [FileInfo](../com.groupdocs.parser.options/fileinfo) | Representa la información del archivo. |
| [FileType](../com.groupdocs.parser.options/filetype) | Representa el tipo de archivo. |
| [FormattedTextOptions](../com.groupdocs.parser.options/formattedtextoptions) | Proporciona las opciones que se utilizan para la extracción de texto con formato. |
| [HighlightOptions](../com.groupdocs.parser.options/highlightoptions) | Proporciona las opciones que se utilizan para extraer un resaltado (un bloque de texto alrededor del texto encontrado en escenarios de búsqueda). |
| [ImageOptions](../com.groupdocs.parser.options/imageoptions) | Proporciona las opciones que se utilizan para la extracción de imágenes. |
| [LoadOptions](../com.groupdocs.parser.options/loadoptions) | Proporciona las opciones que se utilizan para abrir un archivo. |
| [OcrConnectorBase](../com.groupdocs.parser.options/ocrconnectorbase) | Proporciona la funcionalidad OCR. |
| [OcrEventHandler](../com.groupdocs.parser.options/ocreventhandler) | Proporciona un controlador para eventos OCR. |
| [OcrOptions](../com.groupdocs.parser.options/ocroptions) | Proporciona las opciones que se utilizan para el Conector OCR. |
| [PageAreaOptions](../com.groupdocs.parser.options/pageareaoptions) | Proporciona las opciones que se utilizan para la extracción de áreas de página. |
| [PageInfo](../com.groupdocs.parser.options/pageinfo) | Representa la información de la página del documento. |
| [PageRenderInfo](../com.groupdocs.parser.options/pagerenderinfo) | Representa la información de cómo se renderiza una página. |
| [PageTableAreaOptions](../com.groupdocs.parser.options/pagetableareaoptions) | Proporciona las opciones que se utilizan para la extracción de áreas de tabla de página. |
| [PageTextAreaOptions](../com.groupdocs.parser.options/pagetextareaoptions) | Proporciona las opciones que se utilizan para la extracción de áreas de texto de página. |
| [ParserSettings](../com.groupdocs.parser.options/parsersettings) | Proporciona la configuración que se utiliza para personalizar la extracción de datos. |
| [PreviewOptions](../com.groupdocs.parser.options/previewoptions) | Proporciona opciones para establecer requisitos y delegados de flujo para la generación de vistas previas. |
| [SearchOptions](../com.groupdocs.parser.options/searchoptions) | Proporciona las opciones que se utilizan para la búsqueda de texto. |
| [TextDocumentInfo](../com.groupdocs.parser.options/textdocumentinfo) | Representa la información del documento de texto. |
| [TextOptions](../com.groupdocs.parser.options/textoptions) | Proporciona las opciones que se utilizan para la extracción de texto. |

## Interfaces

| Interfaz | Descripción |
| --- | --- |
| [ICreatePageStream](../com.groupdocs.parser.options/icreatepagestream) | Representa un delegado que devuelve un flujo para escribir los datos de vista previa de la página. |
| [IDocumentInfo](../com.groupdocs.parser.options/idocumentinfo) | Representa la información del documento. |
| [ILogger](../com.groupdocs.parser.options/ilogger) | Define la interfaz de un registrador que se utiliza para registrar eventos y errores durante la extracción de datos. |
| [IPreviewPageRender](../com.groupdocs.parser.options/ipreviewpagerender) | Representa un método que se llama antes de que se renderice una página del documento. |
| [IReleasePageStream](../com.groupdocs.parser.options/ireleasepagestream) | Representa un método que libera el flujo creado por el delegado [ICreatePageStream](../com.groupdocs.parser.options/icreatepagestream). |

## Enumeraciones

| Enumeración | Descripción |
| --- | --- |
| [FileFormat](../com.groupdocs.parser.options/fileformat) | Define un tipo de archivo. |
| [FileTypeDetectionMode](../com.groupdocs.parser.options/filetypedetectionmode) | Define un modo de detección del tipo de archivo. |
| [FormattedTextMode](../com.groupdocs.parser.options/formattedtextmode) | Define un modo de texto formateado. |
| [ImageFormat](../com.groupdocs.parser.options/imageformat) | Define un formato de imagen. |
| [PreviewFormats](../com.groupdocs.parser.options/previewformats) | Representa los formatos de vista previa compatibles. |
| [QualityMode](../com.groupdocs.parser.options/qualitymode) | Define un nivel de calidad. |

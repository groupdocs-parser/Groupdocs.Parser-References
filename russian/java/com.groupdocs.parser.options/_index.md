---
title: "com.groupdocs.parser.options"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Пакет предоставляет классы для указания дополнительных параметров при разборе данных из документов."
type: docs
weight: 15
url: /ru/java/com.groupdocs.parser.options/
---

Пакет предоставляет классы для указания дополнительных параметров при разборе данных из документов.



## Классы

| Класс | Описание |
| --- | --- |
| [BarcodeOptions](../com.groupdocs.parser.options/barcodeoptions) | Предоставляет параметры, используемые для извлечения штрих‑кода. |
| [DocumentInfo](../com.groupdocs.parser.options/documentinfo) | Представляет информацию о документе. |
| [EmailConnection](../com.groupdocs.parser.options/emailconnection) | Представляет информацию о подключении к электронной почте. |
| [EmailEwsConnection](../com.groupdocs.parser.options/emailewsconnection) | Представляет информацию о подключении к электронной почте для протокола EWS. |
| [EmailImapConnection](../com.groupdocs.parser.options/emailimapconnection) | Представляет информацию о подключении к электронной почте для протокола IMAP. |
| [EmailPopConnection](../com.groupdocs.parser.options/emailpopconnection) | Представляет информацию о подключении к электронной почте для протокола POP. |
| [ExternalResourceHandler](../com.groupdocs.parser.options/externalresourcehandler) | Предоставляет обработчик для загрузки внешних ресурсов. |
| [ExternalResourceLoadingArgs](../com.groupdocs.parser.options/externalresourceloadingargs) | Предоставляет данные для метода [ExternalResourceHandler.#onLoading(ExternalResourceLoadingArgs)](../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-). |
| [Features](../com.groupdocs.parser.options/features) | Представляет список поддерживаемых функций. |
| [FileInfo](../com.groupdocs.parser.options/fileinfo) | Представляет информацию о файле. |
| [FileType](../com.groupdocs.parser.options/filetype) | Представляет тип файла. |
| [FormattedTextOptions](../com.groupdocs.parser.options/formattedtextoptions) | Предоставляет параметры, используемые для извлечения форматированного текста. |
| [HighlightOptions](../com.groupdocs.parser.options/highlightoptions) | Предоставляет параметры, используемые для извлечения выделения (блока текста вокруг найденного текста в сценариях поиска). |
| [ImageOptions](../com.groupdocs.parser.options/imageoptions) | Предоставляет параметры, используемые для извлечения изображений. |
| [LoadOptions](../com.groupdocs.parser.options/loadoptions) | Предоставляет параметры, используемые для открытия файла. |
| [OcrConnectorBase](../com.groupdocs.parser.options/ocrconnectorbase) | Предоставляет функциональность OCR. |
| [OcrEventHandler](../com.groupdocs.parser.options/ocreventhandler) | Предоставляет обработчик для событий OCR. |
| [OcrOptions](../com.groupdocs.parser.options/ocroptions) | Предоставляет параметры, используемые для OCR Connector. |
| [PageAreaOptions](../com.groupdocs.parser.options/pageareaoptions) | Предоставляет параметры, используемые для извлечения областей страниц. |
| [PageInfo](../com.groupdocs.parser.options/pageinfo) | Представляет информацию о странице документа. |
| [PageRenderInfo](../com.groupdocs.parser.options/pagerenderinfo) | Представляет информацию о том, как отображается страница. |
| [PageTableAreaOptions](../com.groupdocs.parser.options/pagetableareaoptions) | Предоставляет параметры, используемые для извлечения областей таблиц страниц. |
| [PageTextAreaOptions](../com.groupdocs.parser.options/pagetextareaoptions) | Предоставляет параметры, используемые для извлечения областей текста страниц. |
| [ParserSettings](../com.groupdocs.parser.options/parsersettings) | Предоставляет настройки, используемые для настройки извлечения данных. |
| [PreviewOptions](../com.groupdocs.parser.options/previewoptions) | Предоставляет параметры для установки требований и делегатов потоков при генерации предварительного просмотра. |
| [SearchOptions](../com.groupdocs.parser.options/searchoptions) | Предоставляет параметры, используемые для поиска текста. |
| [TextDocumentInfo](../com.groupdocs.parser.options/textdocumentinfo) | Представляет информацию о текстовом документе. |
| [TextOptions](../com.groupdocs.parser.options/textoptions) | Предоставляет параметры, используемые для извлечения текста. |

## Интерфейсы

| Интерфейс | Описание |
| --- | --- |
| [ICreatePageStream](../com.groupdocs.parser.options/icreatepagestream) | Представляет делегат, который возвращает поток для записи данных предварительного просмотра страницы. |
| [IDocumentInfo](../com.groupdocs.parser.options/idocumentinfo) | Представляет информацию о документе. |
| [ILogger](../com.groupdocs.parser.options/ilogger) | Определяет интерфейс логгера, который используется для записи событий и ошибок во время извлечения данных. |
| [IPreviewPageRender](../com.groupdocs.parser.options/ipreviewpagerender) | Представляет метод, который вызывается перед рендерингом страницы документа. |
| [IReleasePageStream](../com.groupdocs.parser.options/ireleasepagestream) | Представляет метод, который освобождает поток, созданный делегатом [ICreatePageStream](../com.groupdocs.parser.options/icreatepagestream). |

## Перечисления

| Перечисление | Описание |
| --- | --- |
| [FileFormat](../com.groupdocs.parser.options/fileformat) | Определяет тип файла. |
| [FileTypeDetectionMode](../com.groupdocs.parser.options/filetypedetectionmode) | Определяет режим обнаружения типа файла. |
| [FormattedTextMode](../com.groupdocs.parser.options/formattedtextmode) | Определяет режим форматированного текста. |
| [ImageFormat](../com.groupdocs.parser.options/imageformat) | Определяет формат изображения. |
| [PreviewFormats](../com.groupdocs.parser.options/previewformats) | Представляет поддерживаемые форматы предварительного просмотра. |
| [QualityMode](../com.groupdocs.parser.options/qualitymode) | Определяет уровень качества. |

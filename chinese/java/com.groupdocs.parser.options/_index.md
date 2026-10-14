---
title: "com.groupdocs.parser.options"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "该包提供用于在解析文档数据时指定附加选项的类。"
type: docs
weight: 15
url: /zh/java/com.groupdocs.parser.options/
---

该包提供用于在解析文档数据时指定附加选项的类。



## 类

| 类 | 描述 |
| --- | --- |
| [BarcodeOptions](../com.groupdocs.parser.options/barcodeoptions) | 提供用于条形码提取的选项。 |
| [DocumentInfo](../com.groupdocs.parser.options/documentinfo) | 表示文档信息。 |
| [EmailConnection](../com.groupdocs.parser.options/emailconnection) | 表示电子邮件连接信息。 |
| [EmailEwsConnection](../com.groupdocs.parser.options/emailewsconnection) | 表示用于 EWS 协议的电子邮件连接信息。 |
| [EmailImapConnection](../com.groupdocs.parser.options/emailimapconnection) | 表示用于 IMAP 协议的电子邮件连接信息。 |
| [EmailPopConnection](../com.groupdocs.parser.options/emailpopconnection) | 表示用于 POP 协议的电子邮件连接信息。 |
| [ExternalResourceHandler](../com.groupdocs.parser.options/externalresourcehandler) | 提供用于外部资源加载的处理程序。 |
| [ExternalResourceLoadingArgs](../com.groupdocs.parser.options/externalresourceloadingargs) | 提供用于 [ExternalResourceHandler.#onLoading(ExternalResourceLoadingArgs)](../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-) 方法的数据。 |
| [Features](../com.groupdocs.parser.options/features) | 表示受支持的功能列表。 |
| [FileInfo](../com.groupdocs.parser.options/fileinfo) | 表示文件信息。 |
| [FileType](../com.groupdocs.parser.options/filetype) | 表示文件类型。 |
| [FormattedTextOptions](../com.groupdocs.parser.options/formattedtextoptions) | 提供用于格式化文本提取的选项。 |
| [HighlightOptions](../com.groupdocs.parser.options/highlightoptions) | 提供用于提取高亮（在搜索场景中围绕找到的文本的文本块）的选项。 |
| [ImageOptions](../com.groupdocs.parser.options/imageoptions) | 提供用于图像提取的选项。 |
| [LoadOptions](../com.groupdocs.parser.options/loadoptions) | 提供用于打开文件的选项。 |
| [OcrConnectorBase](../com.groupdocs.parser.options/ocrconnectorbase) | 提供 OCR 功能。 |
| [OcrEventHandler](../com.groupdocs.parser.options/ocreventhandler) | 提供用于 OCR 事件的处理程序。 |
| [OcrOptions](../com.groupdocs.parser.options/ocroptions) | 提供用于 OCR Connector 的选项。 |
| [PageAreaOptions](../com.groupdocs.parser.options/pageareaoptions) | 提供用于页面区域提取的选项。 |
| [PageInfo](../com.groupdocs.parser.options/pageinfo) | 表示文档页面信息。 |
| [PageRenderInfo](../com.groupdocs.parser.options/pagerenderinfo) | 表示页面渲染方式的信息。 |
| [PageTableAreaOptions](../com.groupdocs.parser.options/pagetableareaoptions) | 提供用于页面表格区域提取的选项。 |
| [PageTextAreaOptions](../com.groupdocs.parser.options/pagetextareaoptions) | 提供用于页面文本区域提取的选项。 |
| [ParserSettings](../com.groupdocs.parser.options/parsersettings) | 提供用于自定义数据提取的设置。 |
| [PreviewOptions](../com.groupdocs.parser.options/previewoptions) | 提供用于设置预览生成的需求和流委托的选项。 |
| [SearchOptions](../com.groupdocs.parser.options/searchoptions) | 提供用于文本搜索的选项。 |
| [TextDocumentInfo](../com.groupdocs.parser.options/textdocumentinfo) | 表示文本文档信息。 |
| [TextOptions](../com.groupdocs.parser.options/textoptions) | 提供用于文本提取的选项。 |

## 接口

| 接口 | 描述 |
| --- | --- |
| [ICreatePageStream](../com.groupdocs.parser.options/icreatepagestream) | 表示返回用于写入页面预览数据的流的委托。 |
| [IDocumentInfo](../com.groupdocs.parser.options/idocumentinfo) | 表示文档信息。 |
| [ILogger](../com.groupdocs.parser.options/ilogger) | 定义用于在数据提取期间记录事件和错误的日志记录器接口。 |
| [IPreviewPageRender](../com.groupdocs.parser.options/ipreviewpagerender) | 表示在渲染文档页面之前调用的方法。 |
| [IReleasePageStream](../com.groupdocs.parser.options/ireleasepagestream) | 表示释放由 [ICreatePageStream](../com.groupdocs.parser.options/icreatepagestream) 委托创建的流的方法。 |

## 枚举

| 枚举类型 | 描述 |
| --- | --- |
| [FileFormat](../com.groupdocs.parser.options/fileformat) | 定义文件的类型。 |
| [FileTypeDetectionMode](../com.groupdocs.parser.options/filetypedetectionmode) | 定义文件类型检测的模式。 |
| [FormattedTextMode](../com.groupdocs.parser.options/formattedtextmode) | 定义格式化文本模式。 |
| [ImageFormat](../com.groupdocs.parser.options/imageformat) | 定义图像的格式。 |
| [PreviewFormats](../com.groupdocs.parser.options/previewformats) | 表示受支持的预览格式。 |
| [QualityMode](../com.groupdocs.parser.options/qualitymode) | 定义质量级别。 |

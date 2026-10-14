---
title: "com.groupdocs.parser.options"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Paket, belgelerden veri ayrıştırırken ek seçenekleri belirtmek için sınıflar sağlar."
type: docs
weight: 15
url: /tr/java/com.groupdocs.parser.options/
---

Paket, belgelerden veri ayrıştırırken ek seçenekleri belirtmek için sınıflar sağlar.



## Sınıflar

| Sınıf | Açıklama |
| --- | --- |
| [BarcodeOptions](../com.groupdocs.parser.options/barcodeoptions) | Barkod çıkarımı için kullanılan seçenekleri sağlar. |
| [DocumentInfo](../com.groupdocs.parser.options/documentinfo) | Belge bilgisini temsil eder. |
| [EmailConnection](../com.groupdocs.parser.options/emailconnection) | E-posta bağlantı bilgisini temsil eder. |
| [EmailEwsConnection](../com.groupdocs.parser.options/emailewsconnection) | EWS protokolü için e-posta bağlantı bilgisini temsil eder. |
| [EmailImapConnection](../com.groupdocs.parser.options/emailimapconnection) | IMAP protokolü için e-posta bağlantı bilgisini temsil eder. |
| [EmailPopConnection](../com.groupdocs.parser.options/emailpopconnection) | POP protokolü için e-posta bağlantı bilgisini temsil eder. |
| [ExternalResourceHandler](../com.groupdocs.parser.options/externalresourcehandler) | Harici kaynakların yüklenmesi için bir işleyici sağlar. |
| [ExternalResourceLoadingArgs](../com.groupdocs.parser.options/externalresourceloadingargs) | Belirtilen [ExternalResourceHandler.#onLoading(ExternalResourceLoadingArgs)](../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-) yöntemi için verileri sağlar. |
| [Features](../com.groupdocs.parser.options/features) | Desteklenen özellikler listesini temsil eder. |
| [FileInfo](../com.groupdocs.parser.options/fileinfo) | Dosya bilgisini temsil eder. |
| [FileType](../com.groupdocs.parser.options/filetype) | Dosya türünü temsil eder. |
| [FormattedTextOptions](../com.groupdocs.parser.options/formattedtextoptions) | Biçimlendirilmiş metin çıkarımı için kullanılan seçenekleri sağlar. |
| [HighlightOptions](../com.groupdocs.parser.options/highlightoptions) | Vurgulama (arama senaryolarında bulunan metnin etrafındaki metin bloğu) çıkarmak için kullanılan seçenekleri sağlar. |
| [ImageOptions](../com.groupdocs.parser.options/imageoptions) | Görüntü çıkarımı için kullanılan seçenekleri sağlar. |
| [LoadOptions](../com.groupdocs.parser.options/loadoptions) | Bir dosya açmak için kullanılan seçenekleri sağlar. |
| [OcrConnectorBase](../com.groupdocs.parser.options/ocrconnectorbase) | OCR işlevselliğini sağlar. |
| [OcrEventHandler](../com.groupdocs.parser.options/ocreventhandler) | OCR olayları için bir işleyici sağlar. |
| [OcrOptions](../com.groupdocs.parser.options/ocroptions) | OCR Bağlayıcısı için kullanılan seçenekleri sağlar. |
| [PageAreaOptions](../com.groupdocs.parser.options/pageareaoptions) | Sayfa alanı çıkarımı için kullanılan seçenekleri sağlar. |
| [PageInfo](../com.groupdocs.parser.options/pageinfo) | Belge sayfası bilgisini temsil eder. |
| [PageRenderInfo](../com.groupdocs.parser.options/pagerenderinfo) | Bir sayfanın nasıl render edildiği bilgisini temsil eder. |
| [PageTableAreaOptions](../com.groupdocs.parser.options/pagetableareaoptions) | Sayfa tablo alanı çıkarımı için kullanılan seçenekleri sağlar. |
| [PageTextAreaOptions](../com.groupdocs.parser.options/pagetextareaoptions) | Sayfa metin alanı çıkarımı için kullanılan seçenekleri sağlar. |
| [ParserSettings](../com.groupdocs.parser.options/parsersettings) | Veri çıkarımını özelleştirmek için kullanılan ayarları sağlar. |
| [PreviewOptions](../com.groupdocs.parser.options/previewoptions) | Önizleme oluşturma için gereksinimleri ve akış delegelerini ayarlamak üzere seçenekler sağlar. |
| [SearchOptions](../com.groupdocs.parser.options/searchoptions) | Metin araması için kullanılan seçenekleri sağlar. |
| [TextDocumentInfo](../com.groupdocs.parser.options/textdocumentinfo) | Metin belgesi bilgisini temsil eder. |
| [TextOptions](../com.groupdocs.parser.options/textoptions) | Metin çıkarımı için kullanılan seçenekleri sağlar. |

## Arayüzler

| Arayüz | Açıklama |
| --- | --- |
| [ICreatePageStream](../com.groupdocs.parser.options/icreatepagestream) | Sayfa önizleme verilerini yazmak için bir akış döndüren delegeyi temsil eder. |
| [IDocumentInfo](../com.groupdocs.parser.options/idocumentinfo) | Belge bilgisini temsil eder. |
| [ILogger](../com.groupdocs.parser.options/ilogger) | Veri çıkarma sırasında olayları ve hataları kaydetmek için kullanılan bir kaydedicinin arabirimini tanımlar. |
| [IPreviewPageRender](../com.groupdocs.parser.options/ipreviewpagerender) | Bir belge sayfası işlenmeden önce çağrılan bir yöntemi temsil eder. |
| [IReleasePageStream](../com.groupdocs.parser.options/ireleasepagestream) | [ICreatePageStream](../com.groupdocs.parser.options/icreatepagestream) temsilcisi tarafından oluşturulan akışı serbest bırakan bir yöntemi temsil eder. |

## Sınıflandırmalar

| Enum | Açıklama |
| --- | --- |
| [FileFormat](../com.groupdocs.parser.options/fileformat) | Dosyanın bir türünü tanımlar. |
| [FileTypeDetectionMode](../com.groupdocs.parser.options/filetypedetectionmode) | Dosya türü algılamanın bir modunu tanımlar. |
| [FormattedTextMode](../com.groupdocs.parser.options/formattedtextmode) | Biçimlendirilmiş metin modunu tanımlar. |
| [ImageFormat](../com.groupdocs.parser.options/imageformat) | Görselin formatını tanımlar. |
| [PreviewFormats](../com.groupdocs.parser.options/previewformats) | Desteklenen önizleme formatlarını temsil eder. |
| [QualityMode](../com.groupdocs.parser.options/qualitymode) | Kalite seviyesini tanımlar. |

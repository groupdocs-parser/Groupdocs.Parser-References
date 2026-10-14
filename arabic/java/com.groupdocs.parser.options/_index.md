---
title: "com.groupdocs.parser.options"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "توفر الحزمة فئات لتحديد خيارات إضافية عند تحليل البيانات من المستندات."
type: docs
weight: 15
url: /ar/java/com.groupdocs.parser.options/
---

توفر الحزمة فئات لتحديد خيارات إضافية عند تحليل البيانات من المستندات.



## الفئات

| الفئة | الوصف |
| --- | --- |
| [BarcodeOptions](../com.groupdocs.parser.options/barcodeoptions) | يوفر الخيارات التي تُستخدم لاستخراج الباركود. |
| [DocumentInfo](../com.groupdocs.parser.options/documentinfo) | يمثل معلومات المستند. |
| [EmailConnection](../com.groupdocs.parser.options/emailconnection) | يمثل معلومات اتصال البريد الإلكتروني. |
| [EmailEwsConnection](../com.groupdocs.parser.options/emailewsconnection) | يمثل معلومات اتصال البريد الإلكتروني لبروتوكول EWS. |
| [EmailImapConnection](../com.groupdocs.parser.options/emailimapconnection) | يمثل معلومات اتصال البريد الإلكتروني لبروتوكول IMAP. |
| [EmailPopConnection](../com.groupdocs.parser.options/emailpopconnection) | يمثل معلومات اتصال البريد الإلكتروني لبروتوكول POP. |
| [ExternalResourceHandler](../com.groupdocs.parser.options/externalresourcehandler) | يوفر معالجًا لتحميل الموارد الخارجية. |
| [ExternalResourceLoadingArgs](../com.groupdocs.parser.options/externalresourceloadingargs) | يوفر البيانات لطريقة [ExternalResourceHandler.#onLoading(ExternalResourceLoadingArgs)](../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-). |
| [Features](../com.groupdocs.parser.options/features) | يمثل قائمة الميزات المدعومة. |
| [FileInfo](../com.groupdocs.parser.options/fileinfo) | يمثل معلومات الملف. |
| [FileType](../com.groupdocs.parser.options/filetype) | يمثل نوع الملف. |
| [FormattedTextOptions](../com.groupdocs.parser.options/formattedtextoptions) | يوفر الخيارات المستخدمة لاستخراج النص المنسق. |
| [HighlightOptions](../com.groupdocs.parser.options/highlightoptions) | يوفر الخيارات المستخدمة لاستخراج تمييز (كتلة نصية حول النص الموجود في سيناريوهات البحث). |
| [ImageOptions](../com.groupdocs.parser.options/imageoptions) | يوفر الخيارات المستخدمة لاستخراج الصور. |
| [LoadOptions](../com.groupdocs.parser.options/loadoptions) | يوفر الخيارات المستخدمة لفتح ملف. |
| [OcrConnectorBase](../com.groupdocs.parser.options/ocrconnectorbase) | يوفر وظائف OCR. |
| [OcrEventHandler](../com.groupdocs.parser.options/ocreventhandler) | يوفر معالجًا لأحداث OCR. |
| [OcrOptions](../com.groupdocs.parser.options/ocroptions) | يوفر الخيارات المستخدمة لموصل OCR. |
| [PageAreaOptions](../com.groupdocs.parser.options/pageareaoptions) | يوفر الخيارات المستخدمة لاستخراج مناطق الصفحة. |
| [PageInfo](../com.groupdocs.parser.options/pageinfo) | يمثل معلومات صفحة المستند. |
| [PageRenderInfo](../com.groupdocs.parser.options/pagerenderinfo) | يمثل معلومات كيفية عرض الصفحة. |
| [PageTableAreaOptions](../com.groupdocs.parser.options/pagetableareaoptions) | يوفر الخيارات المستخدمة لاستخراج مناطق جداول الصفحة. |
| [PageTextAreaOptions](../com.groupdocs.parser.options/pagetextareaoptions) | يوفر الخيارات المستخدمة لاستخراج مناطق نص الصفحة. |
| [ParserSettings](../com.groupdocs.parser.options/parsersettings) | يوفر الإعدادات المستخدمة لتخصيص استخراج البيانات. |
| [PreviewOptions](../com.groupdocs.parser.options/previewoptions) | يوفر خيارات لتعيين المتطلبات ومندوبين التدفق لإنشاء المعاينة. |
| [SearchOptions](../com.groupdocs.parser.options/searchoptions) | يوفر الخيارات المستخدمة للبحث النصي. |
| [TextDocumentInfo](../com.groupdocs.parser.options/textdocumentinfo) | يمثل معلومات مستند النص. |
| [TextOptions](../com.groupdocs.parser.options/textoptions) | يوفر الخيارات المستخدمة لاستخراج النص. |

## الواجهات

| الواجهة | الوصف |
| --- | --- |
| [ICreatePageStream](../com.groupdocs.parser.options/icreatepagestream) | يمثل مندوبًا يُعيد تدفقًا لكتابة بيانات معاينة الصفحة. |
| [IDocumentInfo](../com.groupdocs.parser.options/idocumentinfo) | يمثل معلومات المستند. |
| [ILogger](../com.groupdocs.parser.options/ilogger) | يحدد واجهة مسجل الأحداث الذي يُستخدم لتسجيل الأحداث والأخطاء أثناء استخراج البيانات. |
| [IPreviewPageRender](../com.groupdocs.parser.options/ipreviewpagerender) | يمثل طريقة تُستدعى قبل عرض صفحة المستند. |
| [IReleasePageStream](../com.groupdocs.parser.options/ireleasepagestream) | يمثل طريقة تُفرج عن الدفق الذي أنشأه المفوض [ICreatePageStream](../com.groupdocs.parser.options/icreatepagestream). |

## التعدادات

| تعداد | الوصف |
| --- | --- |
| [FileFormat](../com.groupdocs.parser.options/fileformat) | يحدد نوع الملف. |
| [FileTypeDetectionMode](../com.groupdocs.parser.options/filetypedetectionmode) | يحدد وضع اكتشاف نوع الملف. |
| [FormattedTextMode](../com.groupdocs.parser.options/formattedtextmode) | يحدد وضع النص المنسق. |
| [ImageFormat](../com.groupdocs.parser.options/imageformat) | يحدد تنسيق الصورة. |
| [PreviewFormats](../com.groupdocs.parser.options/previewformats) | يمثل صيغ المعاينة المدعومة. |
| [QualityMode](../com.groupdocs.parser.options/qualitymode) | يحدد مستوى الجودة. |

---
title: "المحلل"
second_title: "GroupDocs.Parser لـ .NET API مرجع"
description: "يمثل الفئة الرئيسية التي تتحكم في استخراج حاوية صور النص ووظيفة التحليل."
type: docs
weight: 30
url: /ar/net/groupdocs.parser/parser/
---

## Parser class

يمثّل الفئة الرئيسية التي تتحكم في النصوص، الصور، استخراج الحاويات ووظيفة التحليل.

```csharp
public sealed class Parser : IDisposable
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | ينشئ مثيلًا جديدًا للفئة [`Parser`](../parser) لاستخراج البيانات من قاعدة بيانات. |
| [Parser](parser#constructor)(EmailConnection) | ينشئ مثيلًا جديدًا للفئة [`Parser`](../parser) لاستخراج البيانات من خادم بريد إلكتروني بعيد. |
| [Parser](parser#constructor_4)(Stream) | ينشئ مثيلًا جديدًا للفئة [`Parser`](../parser). |
| [Parser](parser#constructor_8)(string) | ينشئ مثيلًا جديدًا للفئة [`Parser`](../parser). |
| [Parser](parser#constructor_12)(Uri) | ينشئ مثيلًا جديدًا للفئة [`Parser`](../parser) لاستخراج البيانات من URI. |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | ينشئ مثيلًا جديدًا للفئة [`Parser`](../parser) لاستخراج البيانات من قاعدة بيانات. |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | ينشئ مثيلًا جديدًا للفئة [`Parser`](../parser) لاستخراج البيانات من خادم بريد إلكتروني بعيد. |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | ينشئ مثيلًا جديدًا للفئة [`Parser`](../parser) مع [`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [Parser](parser#constructor_7)(Stream, ParserSettings) | ينشئ مثيلًا جديدًا للفئة [`Parser`](../parser) مع [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_9)(string, LoadOptions) | ينشئ مثيلًا جديدًا للفئة [`Parser`](../parser) مع [`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [Parser](parser#constructor_11)(string, ParserSettings) | ينشئ مثيلًا جديدًا للفئة [`Parser`](../parser) مع [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_13)(Uri, LoadOptions) | ينشئ مثيلًا جديدًا للفئة [`Parser`](../parser) لاستخراج البيانات من URI مع *loadOptions*. |
| [Parser](parser#constructor_15)(Uri, ParserSettings) | ينشئ مثيلًا جديدًا للفئة [`Parser`](../parser) لاستخراج البيانات من URI مع *parserSettings*. |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | ينشئ مثيلًا جديدًا للفئة [`Parser`](../parser) مع [`LoadOptions`](../../groupdocs.parser.options/loadoptions) و [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_10)(string, LoadOptions, ParserSettings) | ينشئ مثيلًا جديدًا للفئة [`Parser`](../parser) مع [`LoadOptions`](../../groupdocs.parser.options/loadoptions) و [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_14)(Uri, LoadOptions, ParserSettings) | ينشئ مثيلًا جديدًا للفئة [`Parser`](../parser) لاستخراج البيانات من URI مع *loadOptions* و *parserSettings*. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | يحصل على الميزات المدعومة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | ينفّذ مهامًا معرفة من قبل التطبيق مرتبطة بتحرير أو إلغاء أو إعادة ضبط الموارد غير المدارة. |
| [GenerateAdjustmentFields](../../groupdocs.parser/parser/generateadjustmentfields)(AdjustmentFieldsOptions) | ينشئ حقولًا لضبط تلقائي لموضع القالب ومقاسه. |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | احصل على معاينة الصفحات. |
| [GetAnnotations](../../groupdocs.parser/parser/getannotations#getannotations)() | يستخرج التعليقات التوضيحية من المستند. لاحظ أن تنسيق PDF هو الوحيد المدعوم حالياً. |
| [GetAnnotations](../../groupdocs.parser/parser/getannotations#getannotations_1)(int) | يستخرج التعليقات التوضيحية من صفحة المستند. لاحظ أن تنسيق PDF هو الوحيد المدعوم حالياً. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | يستخرج الرموز الشريطية من المستند. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(BarcodeOptions) | يستخرج الرموز الشريطية من المستند باستخدام خيارات التخصيص. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int) | يستخرج الرموز الشريطية من صفحة المستند. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_4)(int, BarcodeOptions) | يستخرج الرموز الشريطية من صفحة المستند باستخدام خيارات التخصيص. |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | يستخرج كائن الحاوية من المستند للعمل مع الصيغ التي تحتوي على مرفقات، أرشيفات ZIP، إلخ. |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | يعيد المعلومات العامة حول المستند. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | يستخرج نصًا منسقًا من المستند. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | يستخرج نصًا منسقًا من صفحة المستند. |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | يستخرج تمييزًا من المستند. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | يستخرج الروابط التشعبية من المستند. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | يستخرج الروابط التشعبية من صفحة المستند. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | يستخرج الروابط التشعبية من المستند باستخدام خيارات التخصيص (لتحديد المنطقة المستطيلة التي تحتوي على الروابط التشعبية). |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | يستخرج الروابط التشعبية من صفحة المستند باستخدام خيارات التخصيص (لتحديد المنطقة المستطيلة التي تحتوي على الروابط التشعبية). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | يستخرج الصور من المستند. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | يستخرج الصور من صفحة المستند. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | يستخرج الصور من المستند باستخدام خيارات التخصيص (لتحديد المنطقة المستطيلة التي تحتوي على الصور). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | يستخرج الصور من صفحة المستند باستخدام خيارات التخصيص (لتحديد المنطقة المستطيلة التي تحتوي على الصور). |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | يستخرج البيانات الوصفية من المستند. |
| [GetPagePreview](../../groupdocs.parser/parser/getpagepreview#getpagepreview)(int) | ينشئ معاينة لصفحة المستند. |
| [GetPagePreview](../../groupdocs.parser/parser/getpagepreview#getpagepreview_1)(int, PagePreviewOptions) | ينشئ معاينة لصفحة المستند باستخدام خيارات التخصيص. |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | يستخرج نصًا منظمًا من المستند. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)() | يستخرج الجداول من المستند. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_2)(int) | يستخرج الجداول من صفحة المستند. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(PageTableAreaOptions) | يستخرج الجداول من المستند. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_3)(int, PageTableAreaOptions) | يستخرج الجداول من صفحة المستند. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | يستخرج نصًا من المستند. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | يستخرج نصًا من صفحة المستند. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | يستخرج صفحة نصية من المستند باستخدام خيارات النص (لتمكين وضع استخراج النص الخام السريع). |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | يستخرج نصًا من صفحة المستند باستخدام خيارات النص (لتمكين وضع استخراج النص الخام السريع). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | يستخرج مناطق النص من المستند. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | يستخرج مناطق النص من صفحة المستند. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | يستخرج مناطق النص من المستند باستخدام خيارات التخصيص (التعبير النمطي، مطابقة الحالة، إلخ). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | يستخرج مناطق النص من صفحة المستند باستخدام خيارات التخصيص (التعبير النمطي، مطابقة الحالة، إلخ). |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | يستخرج جدول المحتويات من المستند. |
| [GetWorksheetCells](../../groupdocs.parser/parser/getworksheetcells#getworksheetcells)(int) | يستخرج خلايا ورقة العمل. |
| [GetWorksheetCells](../../groupdocs.parser/parser/getworksheetcells#getworksheetcells_1)(int, WorksheetOptions) | يستخرج خلايا ورقة العمل باستخدام خيارات التخصيص. |
| [GetWorksheetInfo](../../groupdocs.parser/parser/getworksheetinfo#getworksheetinfo_1)() | يستخرج المعلومات حول جميع أوراق العمل في جدول البيانات. |
| [GetWorksheetInfo](../../groupdocs.parser/parser/getworksheetinfo#getworksheetinfo)(int) | يستخرج المعلومات حول ورقة العمل. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate)(Template) | يقوم بتحليل المستند باستخدام القالب الذي أنشأه المستخدم. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate_1)(Template, ParseByTemplateOptions) | يقوم بتحليل المستند باستخدام القالب الذي أنشأه المستخدم باستخدام خيارات التخصيص. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate_2)(TemplateCollection, ParseByTemplateOptions) | يختار القالب الأنسب من المجموعة المقدمة ثم يحلل المستند وفقًا للقالب المختار. |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | يقوم بتحليل نموذج المستند. |
| [Search](../../groupdocs.parser/parser/search#search)(string) | يبحث عن *keyword* في المستند. |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | يبحث عن *keyword* في المستند باستخدام خيارات البحث (التعبير النمطي، مطابقة الحالة، إلخ). |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | يعيد المعلومات العامة حول الملف. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | يعيد المعلومات العامة حول الملف. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | يعيد المعلومات العامة حول الملف. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | يعيد المعلومات العامة حول الملف. |

### انظر أيضًا

* namespace [GroupDocs.Parser](../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

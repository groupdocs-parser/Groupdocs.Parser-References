---
title: Parser
second_title: GroupDocs.Parser لمرجع .NET API
description: يمثل الفئة الرئيسية التي تتحكم في النصوص والصور ووظائف استخراج الحاوية والتحليل.
type: docs
weight: 640
url: /ar/net/groupdocs.parser/parser/
---
## Parser class

يمثل الفئة الرئيسية التي تتحكم في النصوص والصور ووظائف استخراج الحاوية والتحليل.

```csharp
public sealed class Parser : IDisposable
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | يقوم بتهيئة مثيل جديد لملف[`Parser`](../parser) فئة لاستخراج البيانات من قاعدة بيانات. |
| [Parser](parser#constructor)(EmailConnection) | يقوم بتهيئة مثيل جديد لملف[`Parser`](../parser) فئة لاستخراج البيانات من خادم بريد إلكتروني بعيد. |
| [Parser](parser#constructor_4)(Stream) | يقوم بتهيئة مثيل جديد لملف[`Parser`](../parser) فئة . |
| [Parser](parser#constructor_8)(string) | يقوم بتهيئة مثيل جديد لملف[`Parser`](../parser) فئة . |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | يقوم بتهيئة مثيل جديد لملف[`Parser`](../parser) فئة لاستخراج البيانات من قاعدة بيانات. |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | يقوم بتهيئة مثيل جديد لملف[`Parser`](../parser) فئة لاستخراج البيانات من خادم بريد إلكتروني بعيد. |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | يقوم بتهيئة مثيل جديد لملف[`Parser`](../parser) فئة مع[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_7)(Stream, ParserSettings) | يقوم بتهيئة مثيل جديد لملف[`Parser`](../parser) فئة مع[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_9)(string, LoadOptions) | يقوم بتهيئة مثيل جديد لملف[`Parser`](../parser) فئة مع[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_11)(string, ParserSettings) | يقوم بتهيئة مثيل جديد لملف[`Parser`](../parser) فئة مع[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | يقوم بتهيئة مثيل جديد لملف[`Parser`](../parser) فئة مع[`LoadOptions`](../../groupdocs.parser.options/loadoptions) و[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_10)(string, LoadOptions, ParserSettings) | يقوم بتهيئة مثيل جديد لملف[`Parser`](../parser) فئة مع[`LoadOptions`](../../groupdocs.parser.options/loadoptions) و[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |

## الخصائص

| اسم | وصف |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | الحصول على الميزات المدعومة . |

## طُرق

| اسم | وصف |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | تنفيذ مهام محددة بواسطة التطبيق مرتبطة بتحرير الموارد غير المُدارة أو تحريرها أو إعادة تعيينها. |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | الحصول على معاينة للصفحات . |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | استخراج الرموز الشريطية من المستند. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_2)(int) | استخراج الرموز الشريطية من صفحة المستند. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(PageAreaOptions) | استخراج الرموز الشريطية من المستند باستخدام خيارات التخصيص (لتعيين المنطقة المستطيلة التي تحتوي على رموز شريطية) . |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int, PageAreaOptions) | استخراج الرموز الشريطية من صفحة المستند باستخدام خيارات التخصيص (لتعيين المنطقة المستطيلة التي تحتوي على رموز شريطية) . |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | استخراج كائن حاوية من المستند للعمل مع التنسيقات التي تحتوي على مرفقات وأرشيفات ZIP وما إلى ذلك. |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | إرجاع المعلومات العامة حول المستند. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | استخراج نص منسق من المستند. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | استخراج نص منسق من صفحة المستند. |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | لاستخراج تمييز من المستند. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | استخراج الارتباطات التشعبية من المستند. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | استخراج الارتباطات التشعبية من صفحة المستند. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | استخراج الارتباطات التشعبية من المستند باستخدام خيارات التخصيص (لتعيين المنطقة المستطيلة التي تحتوي على ارتباطات تشعبية) . |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | استخراج الارتباطات التشعبية من صفحة المستند باستخدام خيارات التخصيص (لتعيين المنطقة المستطيلة التي تحتوي على ارتباطات تشعبية) . |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | استخراج الصور من المستند. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | استخراج الصور من صفحة المستند. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | استخراج الصور من المستند باستخدام خيارات التخصيص (لتعيين المنطقة المستطيلة التي تحتوي على الصور) . |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | استخراج الصور من صفحة المستند باستخدام خيارات التخصيص (لتعيين المنطقة المستطيلة التي تحتوي على الصور) . |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | استخراج البيانات الوصفية من المستند. |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | استخراج نص منظم من المستند. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)(PageTableAreaOptions) | استخراج الجداول من المستند. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(int, PageTableAreaOptions) | استخراج الجداول من صفحة المستند. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | استخراج نص من المستند. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | استخراج نص من صفحة المستند. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | استخراج صفحة نصية من المستند باستخدام خيارات النص (لتمكين وضع الاستخراج السريع للنص الخام) . |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | استخراج نص من صفحة المستند باستخدام خيارات النص (لتمكين وضع الاستخراج السريع للنص الخام) . |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | استخراج مناطق النص من المستند. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | استخراج مناطق النص من صفحة المستند. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | استخراج مناطق النص من المستند باستخدام خيارات التخصيص (التعبير العادي ، حالة المطابقة ، إلخ.) . |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | استخراج مناطق النص من صفحة المستند باستخدام خيارات التخصيص (التعبير العادي ، حالة المطابقة ، إلخ.) . |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | استخراج جدول محتويات من المستند. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate)(Template) | يوزع المستند بواسطة القالب الذي تم إنشاؤه بواسطة المستخدم. |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | توزيع نموذج المستند. |
| [Search](../../groupdocs.parser/parser/search#search)(string) | عمليات البحث أ*keyword* في المستند. |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | عمليات البحث أ*keyword*في المستند باستخدام خيارات البحث (التعبير العادي ، حالة المطابقة ، إلخ.) . |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | إرجاع المعلومات العامة حول ملف . |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | إرجاع المعلومات العامة حول ملف . |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | إرجاع المعلومات العامة حول ملف . |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | إرجاع المعلومات العامة حول ملف . |

### أنظر أيضا

* مساحة الاسم [GroupDocs.Parser](../../groupdocs.parser)
* المجسم [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

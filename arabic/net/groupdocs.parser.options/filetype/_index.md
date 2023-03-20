---
title: FileType
second_title: GroupDocs.Parser لمرجع .NET API
description: يمثل نوع الملف. يوفر طرقًا للحصول على قائمة بجميع أنواع الملفات التي يدعمهاGroupDocs.Parser .
type: docs
weight: 380
url: /ar/net/groupdocs.parser.options/filetype/
---
## FileType class

يمثل نوع الملف. يوفر طرقًا للحصول على قائمة بجميع أنواع الملفات التي يدعمها**GroupDocs.Parser** .

```csharp
public sealed class FileType : IEquatable<FileType>
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [Extension](../../groupdocs.parser.options/filetype/extension) { get; } | لاحقة اسم الملف (بما في ذلك النقطة ".") مثل ".doc" . |
| [FileFormat](../../groupdocs.parser.options/filetype/fileformat) { get; } | اسم نوع الملف ، مثل "مستند Microsoft Word". |
| [Format](../../groupdocs.parser.options/filetype/format) { get; } | تنسيق الملف ، مثل "معالجة الكلمات". |

## طُرق

| اسم | وصف |
| --- | --- |
| static [FromExtension](../../groupdocs.parser.options/filetype/fromextension)(string) | امتداد ملف الخرائط لنوع الملف. |
| [Equals](../../groupdocs.parser.options/filetype/equals#equals)(FileType) | يحدد ما إذا كان التيار[`FileType`](../filetype) هو نفسه كما هو محدد[`FileType`](../filetype) الكائن . |
| override [Equals](../../groupdocs.parser.options/filetype/equals#equals_1)(object) | يحدد ما إذا كان التيار[`FileType`](../filetype) هو نفس الكائن المحدد. |
| override [GetHashCode](../../groupdocs.parser.options/filetype/gethashcode)() | إرجاع كود التجزئة الحالي[`FileType`](../filetype) الكائن . |
| override [ToString](../../groupdocs.parser.options/filetype/tostring)() | إرجاع سلسلة تمثل الكائن الحالي. |
| static [GetSupportedFileTypes](../../groupdocs.parser.options/filetype/getsupportedfiletypes)() | استرداد أنواع الملفات المدعومة |
| [operator ==](../../groupdocs.parser.options/filetype/op_equality) | تحديد ما إذا كان اثنان[`FileType`](../filetype) الكائنات هي نفسها. |
| [operator !=](../../groupdocs.parser.options/filetype/op_inequality) | تحديد ما إذا كان اثنان[`FileType`](../filetype) الكائنات ليست هي نفسها. |

## مجالات

| اسم | وصف |
| --- | --- |
| static readonly [BMP](../../groupdocs.parser.options/filetype/bmp) | الملفات ذات الامتداد .BMP تمثل ملفات الصور النقطية المستخدمة لتخزين الصور الرقمية. تعرف على المزيد حول تنسيق الملف هذا[هنا](https://wiki.fileformat.com/image/bmp/) . |
| static readonly [BZ2](../../groupdocs.parser.options/filetype/bz2) | ملف مضغوط باستخدام خوارزمية Bzip2 . |
| static readonly [CGM](../../groupdocs.parser.options/filetype/cgm) | Computer Graphics Metafile (CGM) هو تنسيق مجاني ، مستقل عن النظام الأساسي ، ومعيار دولي metafile لتخزين وتبادل الرسومات المتجهة (2D) والرسومات النقطية والنص . تعرف على المزيد حول تنسيق الملف هذا [هنا](https://wiki.fileformat.com/page-description-language/cgm/) . |
| static readonly [CHM](../../groupdocs.parser.options/filetype/chm) | يمثل تنسيق ملف CHM ملف تعليمات Microsoft HTML الذي يتكون من مجموعة من صفحات HTML . تعرف على المزيد حول تنسيق الملف هذا [هنا](https://wiki.fileformat.com/web/chm/) . |
| static readonly [CSV](../../groupdocs.parser.options/filetype/csv) | تمثل الملفات ذات الامتداد CSV (قيم مفصولة بفواصل) ملفات النص العادي التي تحتوي على سجلات البيانات بقيم مفصولة بفواصل. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/spreadsheet/csv/) . |
| static readonly [DCM](../../groupdocs.parser.options/filetype/dcm) | تمثل الملفات ذات الامتداد .DCM الصورة الرقمية التي تخزن المعلومات الطبية للمرضى مثل التصوير بالرنين المغناطيسي والأشعة المقطعية وصور الموجات فوق الصوتية . تعرف على المزيد حول تنسيق الملف هذا [هنا](https://wiki.fileformat.com/image/dcm/) . |
| static readonly [DIB](../../groupdocs.parser.options/filetype/dib) | ملف DIB (صورة نقطية مستقلة عن الجهاز) هو ملف صورة نقطية مشابه في البنية لملفات الصور النقطية القياسية (BMP) ولكن له رأس مختلف. تعرف على المزيد حول تنسيق الملف هذا [هنا](https://wiki.fileformat.com/image/dib/) . |
| static readonly [DJVU](../../groupdocs.parser.options/filetype/djvu) | DjVu ، يُنطق باسم "déjà vu" ، وهو تنسيق ملف رسومي مخصص للمستندات الممسوحة ضوئيًا والكتب خاصة تلك التي تحتوي على مجموعة من النصوص والرسومات والصور والصور الفوتوغرافية. تعرف على المزيد حول تنسيق الملف هذا[هنا](https://wiki.fileformat.com/image/djvu/) . |
| static readonly [DOC](../../groupdocs.parser.options/filetype/doc) | تمثل الملفات ذات الامتداد .doc المستندات التي تم إنشاؤها بواسطة Microsoft Word أو مستندات معالجة النصوص الأخرى بتنسيق ملف ثنائي. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/word-processing/doc/) . |
| static readonly [DOCM](../../groupdocs.parser.options/filetype/docm) | ملفات DOCM هي Microsoft Word 2007 أو مستندات تم إنشاؤها بأعلى مع إمكانية تشغيل وحدات الماكرو. تعرف على المزيد حول تنسيق الملف هذا[هنا](https://wiki.fileformat.com/word-processing/docm/) . |
| static readonly [DOCX](../../groupdocs.parser.options/filetype/docx) | DOCX هو تنسيق معروف لمستندات Microsoft Word. تم تقديمه من عام 2007 مع الإصدار من Microsoft Office 2007 ، تم تغيير هيكل تنسيق المستند الجديد هذا من عادي binary إلى مجموعة من ملفات XML والملفات الثنائية. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/word-processing/docx/) . |
| static readonly [DOT](../../groupdocs.parser.options/filetype/dot) | الملفات ذات الامتداد .DOT هي ملفات قوالب تم إنشاؤها بواسطة Microsoft Word للحصول على إعدادات مهيأة مسبقًا لتوليد المزيد من ملفات DOC أو DOCX. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/word-processing/dot/) . |
| static readonly [DOTM](../../groupdocs.parser.options/filetype/dotm) | يمثل ملف بامتداد DOTM ملف قالب تم إنشاؤه باستخدام Microsoft Word 2007 أو أعلى . تعرف على المزيد حول تنسيق الملف هذا[هنا](https://wiki.fileformat.com/word-processing/dotm/) . |
| static readonly [DOTX](../../groupdocs.parser.options/filetype/dotx) | الملفات ذات امتداد DOTX هي ملفات قوالب تم إنشاؤها بواسطة Microsoft Word للحصول على إعدادات مهيأة مسبقًا لتوليد المزيد من ملفات DOCX. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/word-processing/dotx/) . |
| static readonly [EMF](../../groupdocs.parser.options/filetype/emf) | يخزن تنسيق ملف التعريف المحسن (EMF) الصور الرسومية بشكل مستقل عن الجهاز. تعرف على المزيد حول تنسيق الملف هذا [هنا](https://wiki.fileformat.com/image/emf/) . |
| static readonly [EML](../../groupdocs.parser.options/filetype/eml) | يمثل تنسيق ملف EML رسائل البريد الإلكتروني المحفوظة باستخدام Outlook والتطبيقات الأخرى ذات الصلة. تعرف على المزيد حول تنسيق الملف هذا[هنا](https://wiki.fileformat.com/email/eml/) . |
| static readonly [EMLX](../../groupdocs.parser.options/filetype/emlx) | تم تنفيذ وتطوير تنسيق ملف EMLX بواسطة Apple. يستخدم تطبيق Apple Mail تنسيق ملف EMLX لتصدير رسائل البريد الإلكتروني. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/email/emlx/) . |
| static readonly [EPS](../../groupdocs.parser.options/filetype/eps) | تصف الملفات ذات امتداد EPS بشكل أساسي برنامج لغة Encapsulated PostScript الذي يصف مظهر صفحة واحدة. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/page-description-language/eps/) . |
| static readonly [EPUB](../../groupdocs.parser.options/filetype/epub) | الملفات ذات الامتداد .EPUB هي تنسيق ملف كتاب إلكتروني يوفر تنسيق منشور رقمي قياسي للناشرين والمستهلكين. تعرف على المزيد حول تنسيق الملف هذا [هنا](https://wiki.fileformat.com/ebook/epub/) . |
| static readonly [FB2](../../groupdocs.parser.options/filetype/fb2) | الملفات ذات الامتداد FB2 هي ملفات FictionBook 2.0 eBook التي تحتوي على بنية الكتاب الإلكتروني . تعرف على المزيد حول تنسيق الملف هذا [هنا](https://wiki.fileformat.com/ebook/fb2/) . |
| static readonly [GIF](../../groupdocs.parser.options/filetype/gif) | تنسيق GIF أو Graphical Interchange Format هو نوع من الصور المضغوطة بشدة. تعرف على المزيد حول تنسيق الملف هذا[هنا](https://wiki.fileformat.com/image/gif/) . |
| static readonly [GZ](../../groupdocs.parser.options/filetype/gz) | الملفات ذات الامتداد .gz هي ملفات مضغوطة تم إنشاؤها باستخدام تطبيق ضغط gzip . تعرف على المزيد حول تنسيق الملف هذا [هنا](https://wiki.fileformat.com/compression/gz/) . |
| static readonly [HTM](../../groupdocs.parser.options/filetype/htm) | تمثل الملفات ذات الامتداد HTM لغة ترميز النص التشعبي لإنشاء صفحات الويب للعرض في متصفحات الويب مثل Google Chrome و Internet Explorer و Firefox وعدد آخر. تعرف على المزيد حول تنسيق الملف هذا [هنا](https://wiki.fileformat.com/web/htm/) . |
| static readonly [HTML](../../groupdocs.parser.options/filetype/html) | HTML (لغة ترميز النص التشعبي) هي امتداد لصفحات الويب التي تم إنشاؤها للعرض في المتصفحات . تعرف على المزيد حول تنسيق الملف هذا [هنا](https://wiki.fileformat.com/web/html/) . |
| static readonly [ICO](../../groupdocs.parser.options/filetype/ico) | الملفات ذات الامتداد ICO هي أنواع ملفات الصور المستخدمة كأيقونة لتمثيل تطبيق على Microsoft Windows . تعرف على المزيد حول تنسيق الملف هذا[هنا](https://wiki.fileformat.com/image/ico/) . |
| static readonly [J2C](../../groupdocs.parser.options/filetype/j2c) | JPEG 2000 (J2C) هو نظام ترميز للصور وأحدث معايير ضغط الصور. تم تصميمه ، باستخدام تقنية المويجات ، يمكن لـ JPEG 2000 ترميز المحتوى غير المفقود بأي جودة في وقت واحد. تعرف على المزيد حول تنسيق الملف هذا[هنا](https://wiki.fileformat.com/image/jp2/) . |
| static readonly [J2K](../../groupdocs.parser.options/filetype/j2k) | JPEG 2000 (J2K) هو نظام ترميز للصور وأحدث معايير ضغط الصور. تم تصميمه ، باستخدام تقنية المويجات ، يمكن لـ JPEG 2000 ترميز المحتوى غير المفقود بأي جودة في وقت واحد. تعرف على المزيد حول تنسيق الملف هذا[هنا](https://wiki.fileformat.com/image/jp2/) . |
| static readonly [JP2](../../groupdocs.parser.options/filetype/jp2) | JPEG 2000 (JP2) هو نظام ترميز للصور وأحدث معايير ضغط الصور. تعرف على المزيد حول تنسيق الملف هذا[هنا](https://wiki.fileformat.com/image/jp2/) . |
| static readonly [JPC](../../groupdocs.parser.options/filetype/jpc) | JPEG 2000 (JPC) هو نظام ترميز للصور وأحدث معايير ضغط الصور. تم تصميمه ، باستخدام تقنية المويجات ، يمكن لـ JPEG 2000 ترميز المحتوى غير المفقود بأي جودة في وقت واحد. تعرف على المزيد حول تنسيق الملف هذا[هنا](https://wiki.fileformat.com/image/jp2/) . |
| static readonly [JPEG](../../groupdocs.parser.options/filetype/jpeg) | JPEG هو نوع من تنسيق الصورة يتم حفظه باستخدام طريقة الضغط مع فقد البيانات . تعرف على المزيد حول تنسيق الملف هذا[هنا](https://wiki.fileformat.com/image/jpeg/) . |
| static readonly [JPF](../../groupdocs.parser.options/filetype/jpf) | JPEG 2000 (JPF) هو نظام ترميز للصور وأحدث معايير ضغط الصور. تم تصميمه ، باستخدام تقنية المويجات ، يمكن لـ JPEG 2000 ترميز المحتوى غير المفقود بأي جودة في وقت واحد. تعرف على المزيد حول تنسيق الملف هذا[هنا](https://wiki.fileformat.com/image/jp2/) . |
| static readonly [JPG](../../groupdocs.parser.options/filetype/jpg) | JPG هو نوع من تنسيق الصورة يتم حفظه باستخدام طريقة الضغط مع فقدان البيانات . تعرف على المزيد حول تنسيق الملف هذا[هنا](https://wiki.fileformat.com/image/jpeg/) . |
| static readonly [JPM](../../groupdocs.parser.options/filetype/jpm) | JPEG 2000 (JPM) هو نظام ترميز للصور وأحدث معايير ضغط الصور. تم تصميمه ، باستخدام تقنية المويجات ، يمكن لـ JPEG 2000 ترميز المحتوى غير المفقود بأي جودة في وقت واحد. تعرف على المزيد حول تنسيق الملف هذا[هنا](https://wiki.fileformat.com/image/jp2/) . |
| static readonly [JPX](../../groupdocs.parser.options/filetype/jpx) | JPEG 2000 (JPX) هو نظام ترميز للصور وأحدث معايير ضغط الصور. تم تصميمه ، باستخدام تقنية المويجات ، يمكن لـ JPEG 2000 ترميز المحتوى غير المفقود بأي جودة في وقت واحد. تعرف على المزيد حول تنسيق الملف هذا[هنا](https://wiki.fileformat.com/image/jp2/) . |
| static readonly [MD](../../groupdocs.parser.options/filetype/md) | يتم حفظ الملفات النصية التي تم إنشاؤها باستخدام لهجات لغة Markdown بامتداد الملف .MD أو .MARKDOWN. تعرف على المزيد حول تنسيق الملف هذا [هنا](https://wiki.fileformat.com/word-processing/md/) . |
| static readonly [MHT](../../groupdocs.parser.options/filetype/mht) | تمثل الملفات ذات الامتداد MHT تنسيق أرشيف لصفحة الويب يمكن إنشاؤه بواسطة عدد من التطبيقات المختلفة. تعرف على المزيد حول تنسيق الملف هذا [هنا](https://wiki.fileformat.com/web/mhtml/) . |
| static readonly [MHTML](../../groupdocs.parser.options/filetype/mhtml) | تمثل الملفات ذات الامتداد MHTML تنسيق أرشيف لصفحة الويب يمكن إنشاؤه بواسطة عدد من التطبيقات المختلفة. تعرف على المزيد حول تنسيق الملف هذا [هنا](https://wiki.fileformat.com/web/mhtml/) . |
| static readonly [MSG](../../groupdocs.parser.options/filetype/msg) | MSG هو تنسيق ملف يستخدمه Microsoft Outlook و Exchange لتخزين رسائل البريد الإلكتروني أو جهات الاتصال أو موعد أو مهام أخرى. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/email/msg/) . |
| static readonly [NUMBERS](../../groupdocs.parser.options/filetype/numbers) | الملفات التي تحتوي على ملحق ملف .numbers هي ملفات تم إنشاؤها بواسطة تطبيق جداول بيانات Apple iWork Numbers . |
| static readonly [ODG](../../groupdocs.parser.options/filetype/odg) | يتم استخدام تنسيق ملف ODG بواسطة تطبيق رسم Apache OpenOffice لتخزين عناصر الرسم كصورة متجهة. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/image/odg/) . |
| static readonly [ODP](../../groupdocs.parser.options/filetype/odp) | تمثل الملفات ذات الامتداد ODP تنسيق ملف العرض الذي يستخدمه OpenOffice.org في معيار OASISOpen. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/presentation/odp/) . |
| static readonly [ODS](../../groupdocs.parser.options/filetype/ods) | الملفات ذات الحامل بامتداد ODS لتنسيق OpenDocument Spreadsheet Document الذي يمكن تحريره من قبل المستخدم.[هنا](https://wiki.fileformat.com/spreadsheet/ods/) . |
| static readonly [ODT](../../groupdocs.parser.options/filetype/odt) | ملفات ODT هي نوع من المستندات التي تم إنشاؤها باستخدام تطبيقات معالجة الكلمات التي تعتمد على تنسيق OpenDocument Text File. يتم إنشاؤها باستخدام تطبيقات معالج الكلمات مثل OpenOffice Writer و يمكنه الاحتفاظ بمحتوى مثل النص والصور والكائنات والأنماط. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/word-processing/odt/) . |
| static readonly [ONE](../../groupdocs.parser.options/filetype/one) | يتم إنشاء الملف الذي يتم تمثيله بملحق .ONE بواسطة تطبيق Microsoft OneNote . تعرف على المزيد حول تنسيق الملف هذا [هنا](https://wiki.fileformat.com/note-taking/one/) . |
| static readonly [OST](../../groupdocs.parser.options/filetype/ost) | تمثل ملفات OST أو Offline Storage بيانات صندوق بريد المستخدم في وضع عدم الاتصال على الجهاز المحلي عند تسجيل مع Exchange Server باستخدام Microsoft Outlook. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/email/ost/) |
| static readonly [OTP](../../groupdocs.parser.options/filetype/otp) | تمثل الملفات ذات الامتداد .OTP ملفات قالب العرض التي تم إنشاؤها بواسطة التطبيقات بتنسيق OASIS OpenDocument القياسي. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/presentation/otp/) . |
| static readonly [OTS](../../groupdocs.parser.options/filetype/ots) | تحتوي ملفات OTS على ملفات نماذج يستخدمها تطبيق جداول بيانات OpenOffice. |
| static readonly [OTT](../../groupdocs.parser.options/filetype/ott) | تمثل الملفات ذات امتداد OTT مستندات النماذج التي تم إنشاؤها بواسطة التطبيقات بما يتوافق مع تنسيق OpenDocument القياسي من OASIS. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/word-processing/ott/) . |
| static readonly [PCL](../../groupdocs.parser.options/filetype/pcl) | يرمز PCL إلى لغة أوامر الطابعة وهي لغة وصف الصفحة التي تقدمها Hewlett Packard (HP). تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/page-description-language/pcl/) . |
| static readonly [PDF](../../groupdocs.parser.options/filetype/pdf) | تنسيق المستند المحمول (PDF) هو نوع من المستندات التي أنشأتها Adobe في التسعينيات. كان الغرض من تنسيق الملف هذا هو تقديم معيار لتمثيل المستندات والمواد المرجعية الأخرى في تنسيق مستقل عن برامج التطبيقات والأجهزة وكذلك نظام التشغيل. تعرف على المزيد حول تنسيق الملف هذا[هنا](https://wiki.fileformat.com/view/pdf/) . |
| static readonly [PICT](../../groupdocs.parser.options/filetype/pict) | تنسيق ملف PICT هو تنسيق تعريف يمكن استخدامه لكل من الصور النقطية والصور المتجهة. |
| static readonly [PNG](../../groupdocs.parser.options/filetype/png) | PNG ، رسومات الشبكة المحمولة ، يشير إلى نوع من تنسيق ملف الصورة النقطية الذي يستخدم ضغط بدون فقدان . تعرف على المزيد حول تنسيق الملف هذا[هنا](https://wiki.fileformat.com/image/png/) . |
| static readonly [POT](../../groupdocs.parser.options/filetype/pot) | تمثل الملفات ذات الامتداد .POT ملفات قوالب Microsoft PowerPoint التي تم إنشاؤها بواسطة إصدارات PowerPoint 97-2003. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/presentation/pot/) . |
| static readonly [POTM](../../groupdocs.parser.options/filetype/potm) | الملفات ذات الامتداد POTM هي ملفات قوالب Microsoft PowerPoint مع دعم لوحدات الماكرو. يتم إنشاء ملفات POTM باستخدام PowerPoint 2007 أو أعلى وتحتوي على الإعدادات الافتراضية التي يمكن استخدامها لإنشاء ملفات عرض تقديمية أخرى. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/presentation/potm/) . |
| static readonly [POTX](../../groupdocs.parser.options/filetype/potx) | تمثل الملفات ذات الامتداد .POTX عروض تقديمية لقوالب Microsoft PowerPoint التي تم إنشاؤها باستخدام Microsoft PowerPoint 2007 والإصدارات الأحدث. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/presentation/potx/) . |
| static readonly [PPS](../../groupdocs.parser.options/filetype/pps) | PPS ، عرض شرائح PowerPoint ، يتم إنشاء الملفات باستخدام Microsoft PowerPoint لغرض عرض الشرائح. يدعم Microsoft PowerPoint 97-2003 قراءة وإنشاء ملف PPS. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/presentation/pps/) . |
| static readonly [PPSM](../../groupdocs.parser.options/filetype/ppsm) | تمثل الملفات ذات الامتداد PPSM تنسيق ملف عرض الشرائح ممكّن بماكرو تم إنشاؤه باستخدام Microsoft PowerPoint 2007 أو إصدار أحدث. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/presentation/ppsm/) . |
| static readonly [PPSX](../../groupdocs.parser.options/filetype/ppsx) | PPSX ، عرض شرائح Power Point ، يتم إنشاء الملف باستخدام Microsoft PowerPoint 2007 والإصدارات الأحدث لـ غرض عرض الشرائح. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/presentation/ppsx/) . |
| static readonly [PPT](../../groupdocs.parser.options/filetype/ppt) | يمثل ملف بامتداد PPT ملف PowerPoint يتكون من مجموعة من الشرائح لعرضها على هيئة عرض شرائح. تحدد تنسيق الملف الثنائي المستخدم بواسطة Microsoft PowerPoint 97-2003. تعرف على المزيد حول تنسيق الملف هذا[هنا](https://wiki.fileformat.com/presentation/ppt/) . |
| static readonly [PPTM](../../groupdocs.parser.options/filetype/pptm) | الملفات ذات الامتداد PPTM هي ملفات عرض تقديمية تم تمكين الماكرو تم إنشاؤها باستخدام Microsoft PowerPoint 2007 أو الإصدارات الأحدث. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/presentation/pptm/) . |
| static readonly [PPTX](../../groupdocs.parser.options/filetype/pptx) | الملفات ذات امتداد PPTX هي ملفات عرض تقديمي تم إنشاؤها باستخدام تطبيق Microsoft PowerPoint الشهير . على عكس الإصدار السابق من تنسيق ملف العرض التقديمي PPT الذي كان ثنائيًا ، فإن تنسيق PPTX يعتمد على على تنسيق ملف العرض التقديمي XML المفتوح لبرنامج Microsoft PowerPoint. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/presentation/pptx/) . |
| static readonly [PS](../../groupdocs.parser.options/filetype/ps) | PostScript (PS) هي لغة وصف صفحة للأغراض العامة تستخدم في أعمال النشر المكتبي والنشر الإلكتروني. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/page-description-language/ps/) . |
| static readonly [PSD](../../groupdocs.parser.options/filetype/psd) | PSD ، Photoshop Document ، يمثل تنسيق ملف Adobe Photoshop الأصلي المستخدم لتصميم الرسومات وتطويرها. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/image/psd/) . |
| static readonly [PST](../../groupdocs.parser.options/filetype/pst) | تمثل الملفات ذات الامتداد .PST ملفات التخزين الشخصية في Outlook (تسمى أيضًا جدول التخزين الشخصي) التي تخزن مجموعة متنوعة من معلومات المستخدم. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/email/pst/) |
| static readonly [RAR](../../groupdocs.parser.options/filetype/rar) | تمثل الملفات ذات الامتداد .rar ملفات الأرشيف التي تم إنشاؤها لتخزين المعلومات في شكل مضغوط أو عادي . تعرف على المزيد حول تنسيق الملف هذا [هنا](https://wiki.fileformat.com/compression/rar/) . |
| static readonly [RTF](../../groupdocs.parser.options/filetype/rtf) | تم تقديمه وتوثيقه بواسطة Microsoft ، يمثل Rich Text Format (RTF) طريقة لتشفير النص والرسومات المنسقة لاستخدامها في التطبيقات. يسهل التنسيق تبادل document عبر الأنظمة الأساسية مع منتجات Microsoft الأخرى ، وبالتالي يخدم الغرض من قابلية التشغيل البيني. تعرف على المزيد حول تنسيق الملف هذا[هنا](https://wiki.fileformat.com/word-processing/rtf/) . |
| static readonly [SEVENZ](../../groupdocs.parser.options/filetype/sevenz) | 7z هو تنسيق أرشفة لضغط الملفات والمجلدات بنسبة ضغط عالية . تعرف على المزيد حول تنسيق الملف هذا [هنا](https://wiki.fileformat.com/compression/7z/) . |
| static readonly [SVG](../../groupdocs.parser.options/filetype/svg) | ملف SVG هو ملف Scalar Vector Graphics يستخدم تنسيق نص يستند إلى XML لوصف مظهر الصورة. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/page-description-language/svg/) . |
| static readonly [TAR](../../groupdocs.parser.options/filetype/tar) | الملفات ذات الامتداد .tar هي أرشيفات تم إنشاؤها باستخدام الأداة المساعدة المستندة إلى Unix لتجميع ملف واحد أو أكثر . تعرف على المزيد حول تنسيق الملف هذا [هنا](https://wiki.fileformat.com/compression/tar/) . |
| static readonly [TEXT](../../groupdocs.parser.options/filetype/text) | يمثل ملف بامتداد .TEXT مستندًا نصيًا يحتوي على نص عادي في شكل أسطر . تعرف على المزيد حول تنسيق الملف هذا[هنا](https://wiki.fileformat.com/word-processing/txt/) . |
| static readonly [TIF](../../groupdocs.parser.options/filetype/tif) | TIF ، تنسيق ملف الصورة ذي العلامات ، يمثل الصور النقطية المخصصة للاستخدام على مجموعة متنوعة من الأجهزة التي تتوافق مع معيار تنسيق الملف هذا. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/image/tiff/) . |
| static readonly [TIFF](../../groupdocs.parser.options/filetype/tiff) | TIFF ، تنسيق ملف الصورة ذي العلامات ، يمثل الصور النقطية المخصصة للاستخدام على مجموعة متنوعة من الأجهزة التي تتوافق مع معيار تنسيق الملف هذا. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/image/tiff/) . |
| static readonly [TSV](../../groupdocs.parser.options/filetype/tsv) | يمثل تنسيق ملف قيم مفصولة بعلامات جدولة (TSV) بيانات مفصولة بعلامات تبويب بتنسيق نص عادي . تعرف على المزيد حول تنسيق الملف هذا [هنا](https://wiki.fileformat.com/spreadsheet/tsv/) . |
| static readonly [TXT](../../groupdocs.parser.options/filetype/txt) | يمثل ملف بامتداد .TXT مستندًا نصيًا يحتوي على نص عادي في شكل أسطر . تعرف على المزيد حول تنسيق الملف هذا[هنا](https://wiki.fileformat.com/word-processing/txt/) . |
| static readonly [Unknown](../../groupdocs.parser.options/filetype/unknown) | يمثل نوع ملف غير معروف. |
| static readonly [WEBP](../../groupdocs.parser.options/filetype/webp) | WebP ، الذي قدمته Google ، هو تنسيق ملف صورة ويب نقطية حديث يعتمد على ضغط بدون فقدان و . إنه يوفر نفس جودة الصورة مع تقليل حجم الصورة بشكل كبير . تعرف على المزيد حول تنسيق الملف هذا[هنا](https://wiki.fileformat.com/image/webp/) . |
| static readonly [WMF](../../groupdocs.parser.options/filetype/wmf) | الملفات ذات الامتداد WMF تمثل Microsoft Windows Metafile (WMF) لتخزين بيانات المتجهات وكذلك بيانات الصور ذات التنسيق النقطي. تعرف على المزيد حول تنسيق الملف هذا [هنا](https://wiki.fileformat.com/image/wmf/) . |
| static readonly [XHTML](../../groupdocs.parser.options/filetype/xhtml) | XHTML هو تنسيق ملف نصي مع ترميز في XML ، باستخدام إعادة صياغة HTML 4.0. تعرف على المزيد حول تنسيق الملف هذا [هنا](https://wiki.fileformat.com/web/xhtml/) . |
| static readonly [XLA](../../groupdocs.parser.options/filetype/xla) | برنامج Excel 97-2003 الإضافي ، وهو برنامج تكميلي مصمم لتشغيل تعليمات برمجية إضافية. يدعم استخدام مشاريع VBA . |
| static readonly [XLAM](../../groupdocs.parser.options/filetype/xlam) | تنسيق الوظيفة الإضافية المستند إلى XML والممكّن بماكرو ماكرو لبرنامج Excel 2010 و Excel 2007. الوظيفة الإضافية هي برنامج تكميلي مصمم لتشغيل تعليمات برمجية إضافية. يدعم استخدام مشاريع VBA وأوراق ماكرو Excel 4.0 (.xlm). |
| static readonly [XLS](../../groupdocs.parser.options/filetype/xls) | تمثل الملفات ذات الامتداد XLS تنسيق ملف Excel الثنائي. يمكن إنشاء مثل هذه الملفات بواسطة Microsoft Excel بالإضافة إلى برامج جداول البيانات المماثلة الأخرى مثل OpenOffice Calc أو Apple Numbers. تعرف على المزيد حول تنسيق الملف هذا[هنا](https://wiki.fileformat.com/specification/spreadsheet/xls/) . |
| static readonly [XLSB](../../groupdocs.parser.options/filetype/xlsb) | يحدد تنسيق ملف XLSB تنسيق ملف Excel الثنائي ، وهو عبارة عن مجموعة من السجلات والبنى التي تحدد محتوى مصنف Excel. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/specification/spreadsheet/xlsb/) . |
| static readonly [XLSM](../../groupdocs.parser.options/filetype/xlsm) | الملفات ذات الامتداد XLSM هي نوع من ملفات Spreasheet التي تدعم وحدات الماكرو. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/specification/spreadsheet/xlsm/) . |
| static readonly [XLSX](../../groupdocs.parser.options/filetype/xlsx) | XLSX هو تنسيق معروف لمستندات Microsoft Excel تم تقديمه بواسطة Microsoft مع الإصدار من Microsoft Office 2007. تعرف على المزيد حول تنسيق الملف هذا [هنا](https://wiki.fileformat.com/specification/spreadsheet/xlsx/) . |
| static readonly [XLT](../../groupdocs.parser.options/filetype/xlt) | الملفات ذات الامتداد .XLT هي ملفات قوالب تم إنشاؤها باستخدام Microsoft Excel وهو تطبيق spreadsheet الذي يأتي كجزء من مجموعة Microsoft Office. تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/specification/spreadsheet/xlt/) . |
| static readonly [XLTM](../../groupdocs.parser.options/filetype/xltm) | يمثل امتداد الملف XLTM الملفات التي تم إنشاؤها بواسطة Microsoft Excel كملفات قالب تم تمكينها بماكرو . تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/specification/spreadsheet/xltm/) . |
| static readonly [XLTX](../../groupdocs.parser.options/filetype/xltx) | تمثل الملفات ذات الملحق XLTX ملفات قالب Microsoft Excel التي تستند إلى مواصفات تنسيق ملف Office OpenXML . تعرف على المزيد حول هذا الملف format [هنا](https://wiki.fileformat.com/specification/spreadsheet/xltx/) . |
| static readonly [XML](../../groupdocs.parser.options/filetype/xml) | XML تعني لغة التوصيف الموسعة التي تشبه HTML ولكنها تختلف في استخدام العلامات لتعريف الكائنات. تعرف على المزيد حول تنسيق الملف هذا [هنا](https://wiki.fileformat.com/web/xml/) . |
| static readonly [ZIP](../../groupdocs.parser.options/filetype/zip) | يمثل امتداد الملف ZIP أرشيفات يمكنها الاحتفاظ بملف أو مجلد واحد أو أكثر . تعرف على المزيد حول تنسيق الملف هذا [هنا](https://wiki.fileformat.com/compression/zip/) . |

### ملاحظات

**يتعلم أكثر:**

* [تنسيقات المستندات المدعومة](https://docs.groupdocs.com/display/parsernet/Supported+Document+Formats)
* [احصل على تنسيقات الملفات المدعومة](https://docs.groupdocs.com/display/parsernet/Get+supported+file+formats)
* [الحصول على معلومات الوثيقة](https://docs.groupdocs.com/display/parsernet/Get+document+info)

### أنظر أيضا

* مساحة الاسم [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* المجسم [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

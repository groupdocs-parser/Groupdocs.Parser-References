---
title: "FileType"
second_title: "GroupDocs.Parser لـ .NET API مرجع"
description: "يمثل نوع الملف. يوفر طرقًا للحصول على قائمة بجميع أنواع الملفات المدعومة من قبل GroupDocs.Parser."
type: docs
weight: 320
url: /ar/net/groupdocs.parser.options/filetype/
---

## FileType class

يمثل نوع الملف. يوفر طرقًا للحصول على قائمة بجميع أنواع الملفات المدعومة بواسطة **GroupDocs.Parser**.

```csharp
public sealed class FileType : IEquatable<FileType>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Extension](../../groupdocs.parser.options/filetype/extension) { get; } | لاحقة اسم الملف (بما في ذلك النقطة ".") مثال: ".doc". |
| [FileFormat](../../groupdocs.parser.options/filetype/fileformat) { get; } | اسم نوع الملف مثال: "Microsoft Word Document". |
| [Format](../../groupdocs.parser.options/filetype/format) { get; } | تنسيق الملف مثال: "WordProcessing". |

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [FromExtension](../../groupdocs.parser.options/filetype/fromextension)(string) | يربط امتداد الملف بنوع الملف. |
| [Equals](../../groupdocs.parser.options/filetype/equals#equals)(FileType) | يحدد ما إذا كان [`FileType`](../filetype) الحالي هو نفسه كائن [`FileType`](../filetype) المحدد. |
| override [Equals](../../groupdocs.parser.options/filetype/equals#equals_1)(object) | يحدد ما إذا كان [`FileType`](../filetype) الحالي هو نفسه الكائن المحدد. |
| override [GetHashCode](../../groupdocs.parser.options/filetype/gethashcode)() | يرجع رمز التجزئة لكائن [`FileType`](../filetype) الحالي. |
| override [ToString](../../groupdocs.parser.options/filetype/tostring)() | يرجع سلسلة تمثل الكائن الحالي. |
| static [GetSupportedFileTypes](../../groupdocs.parser.options/filetype/getsupportedfiletypes)() | يسترجع أنواع الملفات المدعومة |
| [operator ==](../../groupdocs.parser.options/filetype/op_equality) | يحدد ما إذا كان كائنان [`FileType`](../filetype) متطابقان. |
| [operator !=](../../groupdocs.parser.options/filetype/op_inequality) | يحدد ما إذا كان كائنان [`FileType`](../filetype) غير متطابقين. |

## Fields

| الاسم | الوصف |
| --- | --- |
| static readonly [AZW3](../../groupdocs.parser.options/filetype/azw3) | AZW3، المعروف أيضًا باسم Kindle Format 8 (KF8)، هو النسخة المعدلة من تنسيق ملف الكتاب الإلكتروني AZW المطور لأجهزة Amazon Kindle. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/ebook/azw3/). |
| static readonly [BMP](../../groupdocs.parser.options/filetype/bmp) | الملفات ذات الامتداد .BMP تمثل ملفات صور نقطية تُستخدم لتخزين الصور الرقمية النقطية. هذه الصور مستقلة عن محول الرسومات وتُعرف أيضًا بتنسيق ملف bitmap المستقل عن الجهاز (DIB). تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/image/bmp/). |
| static readonly [BZ2](../../groupdocs.parser.options/filetype/bz2) | ملف مضغوط باستخدام خوارزمية Bzip2. |
| static readonly [CGM](../../groupdocs.parser.options/filetype/cgm) | Computer Graphics Metafile (CGM) هو تنسيق ملف ميتا مجاني، مستقل عن المنصة، معيار دولي لتخزين وتبادل الرسومات المتجهية (2D)، الرسومات النقطية، والنص. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/page-description-language/cgm/). |
| static readonly [CHM](../../groupdocs.parser.options/filetype/chm) | تنسيق ملف CHM يمثل ملف مساعدة HTML من Microsoft يتكون من مجموعة من صفحات HTML. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/web/chm/). |
| static readonly [CSV](../../groupdocs.parser.options/filetype/csv) | الملفات ذات الامتداد CSV (قيم مفصولة بفواصل) تمثل ملفات نصية عادية تحتوي على سجلات بيانات بقيم مفصولة بفواصل. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/spreadsheet/csv/). |
| static readonly [DCM](../../groupdocs.parser.options/filetype/dcm) | الملفات ذات الامتداد .DCM تمثل صورة رقمية تخزن معلومات طبية للمرضى مثل صور الرنين المغناطيسي (MRI)، الأشعة المقطعية (CT) وصور الموجات فوق الصوتية. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/image/dcm/). |
| static readonly [DIB](../../groupdocs.parser.options/filetype/dib) | ملف DIB (Device Independent Bitmap) هو ملف صورة نقطية يشبه في هيكله ملفات Bitmap القياسية (BMP) لكنه يحتوي على رأس مختلف. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/image/dib/). |
| static readonly [DJVU](../../groupdocs.parser.options/filetype/djvu) | DjVu، يُنطق كـ “déjà vu”، هو تنسيق ملف رسومي مخصص للمستندات والكتب الممسوحة ضوئياً، خاصةً تلك التي تحتوي على مزيج من النصوص والرسومات والصور الفوتوغرافية. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/image/djvu/). |
| static readonly [DOC](../../groupdocs.parser.options/filetype/doc) | الملفات ذات الامتداد .doc تمثل مستندات تم إنشاؤها بواسطة Microsoft Word أو برامج معالجة النصوص الأخرى بصيغة ملف ثنائي. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/word-processing/doc/). |
| static readonly [DOCM](../../groupdocs.parser.options/filetype/docm) | ملفات DOCM هي مستندات تم إنشاؤها بواسطة Microsoft Word 2007 أو أحدث وتدعم تشغيل الماكرو. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/word-processing/docm/). |
| static readonly [DOCX](../../groupdocs.parser.options/filetype/docx) | DOCX هو تنسيق معروف لمستندات Microsoft Word. تم تقديمه منذ عام 2007 مع إصدار Microsoft Office 2007، حيث تم تغيير بنية هذا التنسيق الجديد من ثنائي بسيط إلى مزيج من ملفات XML والملفات الثنائية. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/word-processing/docx/). |
| static readonly [DOT](../../groupdocs.parser.options/filetype/dot) | الملفات ذات الامتداد .DOT هي ملفات قالب تم إنشاؤها بواسطة Microsoft Word لتحتوي على إعدادات مسبقة الصياغة لتوليد ملفات DOC أو DOCX لاحقاً. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/word-processing/dot/). |
| static readonly [DOTM](../../groupdocs.parser.options/filetype/dotm) | الملف ذو الامتداد DOTM يمثل ملف قالب تم إنشاؤه باستخدام Microsoft Word 2007 أو أحدث. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/word-processing/dotm/). |
| static readonly [DOTX](../../groupdocs.parser.options/filetype/dotx) | الملفات ذات الامتداد .DOTX هي ملفات قالب تم إنشاؤها بواسطة Microsoft Word لتحتوي على إعدادات مسبقة الصياغة لتوليد ملفات DOCX لاحقاً. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/word-processing/dotx/). |
| static readonly [EMF](../../groupdocs.parser.options/filetype/emf) | تنسيق Enhanced metafile (EMF) يخزن الصور الرسومية بشكل مستقل عن الجهاز. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/image/emf/). |
| static readonly [EML](../../groupdocs.parser.options/filetype/eml) | تنسيق ملف EML يمثل رسائل البريد الإلكتروني المحفوظة باستخدام Outlook وتطبيقات أخرى ذات صلة. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/email/eml/). |
| static readonly [EMLX](../../groupdocs.parser.options/filetype/emlx) | تم تنفيذ وتطوير تنسيق ملف EMLX بواسطة Apple. يستخدم تطبيق Apple Mail تنسيق EMLX لتصدير رسائل البريد الإلكتروني. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/email/emlx/). |
| static readonly [EPS](../../groupdocs.parser.options/filetype/eps) | الملفات ذات الامتداد .EPS تصف أساساً برنامج لغة Encapsulated PostScript الذي يحدد مظهر صفحة واحدة. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/page-description-language/eps/). |
| static readonly [EPUB](../../groupdocs.parser.options/filetype/epub) | الملفات ذات الامتداد .EPUB هي تنسيق ملف إلكتروني يوفر صيغة نشر رقمية قياسية للناشرين والمستهلكين. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/ebook/epub/). |
| static readonly [FB2](../../groupdocs.parser.options/filetype/fb2) | الملفات ذات الامتداد .FB2 هي ملفات eBook من نوع FictionBook 2.0 تحتوي على بنية الكتاب الإلكتروني. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/ebook/fb2/). |
| static readonly [GIF](../../groupdocs.parser.options/filetype/gif) | GIF أو Graphical Interchange Format هو نوع من الصور المضغوطة بشكل كبير. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/image/gif/). |
| static readonly [GZ](../../groupdocs.parser.options/filetype/gz) | الملفات ذات الامتداد .gz هي ملفات مضغوطة تم إنشاؤها باستخدام تطبيق gzip للضغط. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/compression/gz/). |
| static readonly [HTM](../../groupdocs.parser.options/filetype/htm) | الملفات ذات الامتداد .HTM تمثل Hypertext Markup Language لإنشاء صفحات ويب للعرض في متصفحات الويب مثل Google Chrome وInternet Explorer وFirefox والعديد غيرها. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/web/htm/). |
| static readonly [HTML](../../groupdocs.parser.options/filetype/html) | HTML (Hyper Text Markup Language) هو الامتداد الخاص بصفحات الويب التي تُنشأ للعرض في المتصفحات. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/web/html/). |
| static readonly [ICO](../../groupdocs.parser.options/filetype/ico) | الملفات ذات امتداد ICO هي أنواع ملفات صور تُستخدم كأيقونة لتمثيل تطبيق على نظام مايكروسوفت ويندوز. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/image/ico/). |
| static readonly [J2C](../../groupdocs.parser.options/filetype/j2c) | JPEG 2000 (J2C) هو نظام ترميز صور ومعيار ضغط صور متقدم. صُمم باستخدام تقنية الموجة، يمكن لـ JPEG 2000 ترميز محتوى غير فقدان في أي جودة مرة واحدة. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/image/jp2/). |
| static readonly [J2K](../../groupdocs.parser.options/filetype/j2k) | JPEG 2000 (J2K) هو نظام ترميز صور ومعيار ضغط صور متقدم. صُمم باستخدام تقنية الموجة، يمكن لـ JPEG 2000 ترميز محتوى غير فقدان في أي جودة مرة واحدة. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/image/jp2/). |
| static readonly [JP2](../../groupdocs.parser.options/filetype/jp2) | JPEG 2000 (JP2) هو نظام ترميز صور ومعيار ضغط صور متقدم. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/image/jp2/). |
| static readonly [JPC](../../groupdocs.parser.options/filetype/jpc) | JPEG 2000 (JPC) هو نظام ترميز صور ومعيار ضغط صور متقدم. صُمم باستخدام تقنية الموجة، يمكن لـ JPEG 2000 ترميز محتوى غير فقدان في أي جودة مرة واحدة. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/image/jp2/). |
| static readonly [JPEG](../../groupdocs.parser.options/filetype/jpeg) | JPEG هو نوع من تنسيقات الصور يُحفظ باستخدام طريقة الضغط الفاقد. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/image/jpeg/). |
| static readonly [JPF](../../groupdocs.parser.options/filetype/jpf) | JPEG 2000 (JPF) هو نظام ترميز صور ومعيار ضغط صور متقدم. صُمم باستخدام تقنية الموجة، يمكن لـ JPEG 2000 ترميز محتوى غير فقدان في أي جودة مرة واحدة. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/image/jp2/). |
| static readonly [JPG](../../groupdocs.parser.options/filetype/jpg) | JPG هو نوع من تنسيقات الصور يُحفظ باستخدام طريقة الضغط الفاقد. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/image/jpeg/). |
| static readonly [JPM](../../groupdocs.parser.options/filetype/jpm) | JPEG 2000 (JPM) هو نظام ترميز صور ومعيار ضغط صور متقدم. صُمم باستخدام تقنية الموجة، يمكن لـ JPEG 2000 ترميز محتوى غير فقدان في أي جودة مرة واحدة. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/image/jp2/). |
| static readonly [JPX](../../groupdocs.parser.options/filetype/jpx) | JPEG 2000 (JPX) هو نظام ترميز صور ومعيار ضغط صور متقدم. صُمم باستخدام تقنية الموجة، يمكن لـ JPEG 2000 ترميز محتوى غير فقدان في أي جودة مرة واحدة. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/image/jp2/). |
| static readonly [MD](../../groupdocs.parser.options/filetype/md) | ملفات النص التي تُنشأ باستخدام لهجات لغة Markdown تُحفظ بامتداد .MD أو .MARKDOWN. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/word-processing/md/). |
| static readonly [MHT](../../groupdocs.parser.options/filetype/mht) | الملفات ذات امتداد MHT تمثل تنسيق أرشيف صفحة ويب يمكن إنشاؤه بواسطة عدد من التطبيقات المختلفة. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/web/mhtml/). |
| static readonly [MHTML](../../groupdocs.parser.options/filetype/mhtml) | الملفات ذات امتداد MHTML تمثل تنسيق أرشيف صفحة ويب يمكن إنشاؤه بواسطة عدد من التطبيقات المختلفة. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/web/mhtml/). |
| static readonly [MOBI](../../groupdocs.parser.options/filetype/mobi) | تنسيق ملف Mobipocket (في الأصل بامتداد .prc ولاحقًا .mobi) هو تنسيق ثنائي مملوك ومُوثق جزئيًا للكتب الإلكترونية. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/ebook/mobi/). |
| static readonly [MSG](../../groupdocs.parser.options/filetype/msg) | MSG هو تنسيق ملف يستخدمه Microsoft Outlook وExchange لتخزين رسائل البريد الإلكتروني أو جهات الاتصال أو المواعيد أو مهام أخرى. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/email/msg/). |
| static readonly [NUMBERS](../../groupdocs.parser.options/filetype/numbers) | الملفات التي تحمل امتداد .numbers هي ملفات تُنشأ بواسطة تطبيق Apple iWork Numbers لجداول البيانات. |
| static readonly [ODG](../../groupdocs.parser.options/filetype/odg) | تنسيق ملف ODG يُستخدم بواسطة تطبيق Draw في Apache OpenOffice لتخزين عناصر الرسم كصورة متجهة. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/image/odg/). |
| static readonly [ODP](../../groupdocs.parser.options/filetype/odp) | الملفات ذات امتداد ODP تمثل تنسيق ملفات عروض تقديمية يُستخدم من قبل OpenOffice.org في معيار OASISOpen. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/presentation/odp/). |
| static readonly [ODS](../../groupdocs.parser.options/filetype/ods) | الملفات ذات الامتداد ODS تمثل تنسيق مستند جدول بيانات OpenDocument يمكن تحريره من قبل المستخدم. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/spreadsheet/ods/). |
| static readonly [ODT](../../groupdocs.parser.options/filetype/odt) | ملفات ODT هي نوع من المستندات التي تُنشأ باستخدام تطبيقات معالجة النصوص المستندة إلى تنسيق ملف نص OpenDocument. تُنشأ هذه باستخدام تطبيقات معالجة النصوص مثل OpenOffice Writer المجانية ويمكن أن تحتوي على محتوى مثل النصوص، الصور، الكائنات والأنماط. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/word-processing/odt/). |
| static readonly [ONE](../../groupdocs.parser.options/filetype/one) | الملف ذو الامتداد .ONE يتم إنشاؤه بواسطة تطبيق Microsoft OneNote. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/note-taking/one/). |
| static readonly [OST](../../groupdocs.parser.options/filetype/ost) | ملفات OST أو Offline Storage تمثل بيانات صندوق بريد المستخدم في وضع غير متصل على الجهاز المحلي عند التسجيل في Exchange Server باستخدام Microsoft Outlook. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/email/ost/) |
| static readonly [OTP](../../groupdocs.parser.options/filetype/otp) | الملفات ذات الامتداد .OTP تمثل قوالب عروض تقديمية تم إنشاؤها بواسطة تطبيقات بتنسيق معيار OASIS OpenDocument. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/presentation/otp/). |
| static readonly [OTS](../../groupdocs.parser.options/filetype/ots) | ملفات OTS تحتوي على ملفات قوالب تُستخدم بواسطة تطبيق جدول بيانات OpenOffice. |
| static readonly [OTT](../../groupdocs.parser.options/filetype/ott) | الملفات ذات الامتداد OTT تمثل مستندات قوالب تم إنشاؤها بواسطة تطبيقات وفقًا لتنسيق معيار OASIS OpenDocument. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/word-processing/ott/). |
| static readonly [PCL](../../groupdocs.parser.options/filetype/pcl) | PCL تعني لغة أوامر الطابعة وهي لغة وصف الصفحات تم تقديمها من قبل Hewlett Packard (HP). تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/page-description-language/pcl/). |
| static readonly [PDF](../../groupdocs.parser.options/filetype/pdf) | تنسيق المستندات القابل للنقل (PDF) هو نوع من المستندات أنشأته شركة Adobe في تسعينيات القرن الماضي. الهدف من هذا التنسيق هو تقديم معيار لتمثيل المستندات وغيرها من المواد المرجعية بصيغة مستقلة عن برامج التطبيقات، الأجهزة وكذلك نظام التشغيل. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/view/pdf/). |
| static readonly [PICT](../../groupdocs.parser.options/filetype/pict) | تنسيق ملف PICT هو تنسيق ميتا يمكن استخدامه لكل من الصور النقطية (bitmap) والصور المتجهية (vector). |
| static readonly [PNG](../../groupdocs.parser.options/filetype/png) | PNG، Portable Network Graphics، يشير إلى نوع من تنسيقات ملفات الصور النقطية التي تستخدم ضغطًا غير فقدان للبيانات. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/image/png/). |
| static readonly [POT](../../groupdocs.parser.options/filetype/pot) | الملفات ذات الامتداد .POT تمثل قوالب Microsoft PowerPoint التي تم إنشاؤها بواسطة إصدارات PowerPoint 97-2003. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/presentation/pot/). |
| static readonly [POTM](../../groupdocs.parser.options/filetype/potm) | الملفات ذات الامتداد POTM هي قوالب Microsoft PowerPoint التي تدعم الماكرو. يتم إنشاء ملفات POTM باستخدام PowerPoint 2007 أو أحدث وتحتوي على إعدادات افتراضية يمكن استخدامها لإنشاء ملفات عروض تقديمية أخرى. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/presentation/potm/). |
| static readonly [POTX](../../groupdocs.parser.options/filetype/potx) | الملفات ذات الامتداد .POTX تمثل قوالب عروض تقديمية Microsoft PowerPoint التي تم إنشاؤها باستخدام Microsoft PowerPoint 2007 وما فوق. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/presentation/potx/). |
| static readonly [PPS](../../groupdocs.parser.options/filetype/pps) | ملفات PPS، PowerPoint Slide Show، تُنشأ باستخدام Microsoft PowerPoint لأغراض عرض الشرائح. قراءة وإنشاء ملفات PPS مدعومة من قبل Microsoft PowerPoint 97-2003. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/presentation/pps/). |
| static readonly [PPSM](../../groupdocs.parser.options/filetype/ppsm) | الملفات ذات الامتداد PPSM تمثل تنسيق عرض شرائح يدعم الماكرو تم إنشاؤه باستخدام Microsoft PowerPoint 2007 أو أعلى. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/presentation/ppsm/). |
| static readonly [PPSX](../../groupdocs.parser.options/filetype/ppsx) | ملفات PPSX، Power Point Slide Show، تُنشأ باستخدام Microsoft PowerPoint 2007 وما فوق لأغراض عرض الشرائح. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/presentation/ppsx/). |
| static readonly [PPT](../../groupdocs.parser.options/filetype/ppt) | ملف بامتداد PPT يمثل ملف PowerPoint يتكون من مجموعة من الشرائح للعرض كعرض شرائح. يحدد تنسيق الملف الثنائي المستخدم من قبل Microsoft PowerPoint 97-2003. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/presentation/ppt/). |
| static readonly [PPTM](../../groupdocs.parser.options/filetype/pptm) | الملفات ذات الامتداد PPTM هي ملفات عروض تقديمية مدعومة بالماكرو تم إنشاؤها باستخدام Microsoft PowerPoint 2007 أو الإصدارات الأحدث. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/presentation/pptm/). |
| static readonly [PPTX](../../groupdocs.parser.options/filetype/pptx) | الملفات ذات الامتداد PPTX هي ملفات عروض تقديمية تم إنشاؤها باستخدام تطبيق Microsoft PowerPoint الشهير. على عكس نسخة تنسيق ملف العرض التقديمي السابقة PPT التي كانت ثنائية، يعتمد تنسيق PPTX على تنسيق ملف عرض Microsoft PowerPoint المفتوح XML. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/presentation/pptx/). |
| static readonly [PS](../../groupdocs.parser.options/filetype/ps) | PostScript (PS) هي لغة وصف صفحات عامة تُستخدم في مجال النشر المكتبي والإلكتروني. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/page-description-language/ps/). |
| static readonly [PSD](../../groupdocs.parser.options/filetype/psd) | PSD، مستند Photoshop، يمثل تنسيق الملف الأصلي لبرنامج Adobe Photoshop المستخدم في تصميم وتطوير الرسومات. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/image/psd/). |
| static readonly [PST](../../groupdocs.parser.options/filetype/pst) | الملفات ذات الامتداد .PST تمثل ملفات تخزين شخصية لبرنامج Outlook (تُسمى أيضاً جدول التخزين الشخصي) التي تخزن مجموعة متنوعة من معلومات المستخدم. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/email/pst/) |
| static readonly [RAR](../../groupdocs.parser.options/filetype/rar) | الملفات ذات الامتداد .rar تمثل ملفات أرشيفية تم إنشاؤها لتخزين المعلومات بصيغة مضغوطة أو عادية. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/compression/rar/). |
| static readonly [RTF](../../groupdocs.parser.options/filetype/rtf) | تم تقديم وتوثيق Rich Text Format (RTF) من قبل Microsoft، وهو يمثل طريقة لتشفير النص المنسق والرسومات للاستخدام داخل التطبيقات. يسهل هذا التنسيق تبادل المستندات عبر الأنظمة مع منتجات Microsoft الأخرى، وبالتالي يخدم هدف التوافقية. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/word-processing/rtf/). |
| static readonly [SEVENZ](../../groupdocs.parser.options/filetype/sevenz) | 7z هو تنسيق أرشفة لضغط الملفات والمجلدات بنسبة ضغط عالية. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/compression/7z/). |
| static readonly [SVG](../../groupdocs.parser.options/filetype/svg) | ملف SVG هو ملف رسومات متجهية قياسية يستخدم تنسيق نص مبني على XML لوصف مظهر الصورة. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/page-description-language/svg/). |
| static readonly [SVGZ](../../groupdocs.parser.options/filetype/svgz) | ملف SVGZ هو ملف رسومات متجهية قياسية يستخدم تنسيق نص مبني على XML لوصف مظهر الصورة ومضغوط باستخدام ضغط gzip. |
| static readonly [TAR](../../groupdocs.parser.options/filetype/tar) | الملفات ذات الامتداد .tar هي أرشيفات تم إنشاؤها باستخدام أداة تعتمد على Unix لجمع ملف واحد أو أكثر. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/compression/tar/). |
| static readonly [TEXT](../../groupdocs.parser.options/filetype/text) | ملف بامتداد .TEXT يمثل مستند نصي يحتوي على نص عادي على شكل أسطر. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/word-processing/txt/). |
| static readonly [TIF](../../groupdocs.parser.options/filetype/tif) | TIF، تنسيق ملف الصورة الموسومة، يمثل صورًا نقطية مخصصة للاستخدام على مجموعة متنوعة من الأجهزة التي تتوافق مع معيار هذا التنسيق. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/image/tiff/). |
| static readonly [TIFF](../../groupdocs.parser.options/filetype/tiff) | TIFF، تنسيق ملف الصورة الموسومة، يمثل صورًا نقطية مخصصة للاستخدام على مجموعة متنوعة من الأجهزة التي تتوافق مع معيار هذا التنسيق. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/image/tiff/). |
| static readonly [TSV](../../groupdocs.parser.options/filetype/tsv) | تنسيق ملف القيم المفصولة بعلامات جدولة (TSV) يمثل بيانات مفصولة بعلامات جدولة في تنسيق نص عادي. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/spreadsheet/tsv/). |
| static readonly [TXT](../../groupdocs.parser.options/filetype/txt) | ملف بامتداد .TXT يمثل مستند نصي يحتوي على نص عادي على شكل أسطر. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/word-processing/txt/). |
| static readonly [Unknown](../../groupdocs.parser.options/filetype/unknown) | يمثل نوع ملف غير معروف. |
| static readonly [WEBP](../../groupdocs.parser.options/filetype/webp) | WebP، الذي قدمته Google، هو تنسيق ملف صورة ويب نقطية حديث يعتمد على الضغط غير الفاقد والفقدان. يوفر نفس جودة الصورة مع تقليل حجم الصورة بشكل كبير. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/image/webp/). |
| static readonly [WMF](../../groupdocs.parser.options/filetype/wmf) | الملفات ذات امتداد WMF تمثل Microsoft Windows Metafile (WMF) لتخزين البيانات الصورية المتجهة وكذلك بتنسيق bitmap. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/image/wmf/). |
| static readonly [XHTML](../../groupdocs.parser.options/filetype/xhtml) | الـ XHTML هو تنسيق ملف نصي يعتمد على العلامات في XML، باستخدام إعادة صياغة لـ HTML 4.0. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/web/xhtml/). |
| static readonly [XLA](../../groupdocs.parser.options/filetype/xla) | إضافة Excel 97-2003، برنامج إضافي صُمم لتشغيل شفرة إضافية. يدعم استخدام مشاريع VBA. |
| static readonly [XLAM](../../groupdocs.parser.options/filetype/xlam) | تنسيق Add-In القائم على XML والمُمكّن للماكرو لـ Excel 2010 وExcel 2007. الـ Add-In هو برنامج إضافي صُمم لتشغيل شفرة إضافية. يدعم استخدام مشاريع VBA وأوراق ماكرو Excel 4.0 (.xlm). |
| static readonly [XLS](../../groupdocs.parser.options/filetype/xls) | الملفات ذات امتداد XLS تمثل تنسيق ملف Excel الثنائي. يمكن إنشاء مثل هذه الملفات بواسطة Microsoft Excel وكذلك برامج جداول بيانات مشابهة مثل OpenOffice Calc أو Apple Numbers. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/specification/spreadsheet/xls/). |
| static readonly [XLSB](../../groupdocs.parser.options/filetype/xlsb) | تنسيق XLSB يحدد تنسيق ملف Excel الثنائي، وهو مجموعة من السجلات والهياكل التي تحدد محتوى دفتر عمل Excel. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/specification/spreadsheet/xlsb/). |
| static readonly [XLSM](../../groupdocs.parser.options/filetype/xlsm) | الملفات ذات امتداد XLSM هي نوع من ملفات جداول البيانات التي تدعم الماكرو. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/specification/spreadsheet/xlsm/). |
| static readonly [XLSX](../../groupdocs.parser.options/filetype/xlsx) | XLSX هو تنسيق معروف لمستندات Microsoft Excel تم تقديمه من قبل Microsoft مع إصدار Microsoft Office 2007. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/specification/spreadsheet/xlsx/). |
| static readonly [XLT](../../groupdocs.parser.options/filetype/xlt) | الملفات ذات امتداد .XLT هي ملفات قالب تم إنشاؤها باستخدام Microsoft Excel وهو تطبيق جداول بيانات يأتي كجزء من مجموعة Microsoft Office. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/specification/spreadsheet/xlt/). |
| static readonly [XLTM](../../groupdocs.parser.options/filetype/xltm) | امتداد ملف XLTM يمثل الملفات التي تم إنشاؤها بواسطة Microsoft Excel كقوالب مُمكّنة للماكرو. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/specification/spreadsheet/xltm/). |
| static readonly [XLTX](../../groupdocs.parser.options/filetype/xltx) | الملفات ذات امتداد XLTX تمثل ملفات قالب Microsoft Excel المستندة إلى مواصفات تنسيق ملف Office OpenXML. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/specification/spreadsheet/xltx/). |
| static readonly [XML](../../groupdocs.parser.options/filetype/xml) | XML هو اختصار Extensible Markup Language وهو مشابه لـ HTML لكنه مختلف في استخدام العلامات لتعريف الكائنات. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/web/xml/). |
| static readonly [ZIP](../../groupdocs.parser.options/filetype/zip) | امتداد ملف ZIP يمثل أرشيفات يمكنها احتواء ملف أو أكثر أو أدلة. تعرف على المزيد حول هذا التنسيق [هنا](https://wiki.fileformat.com/compression/zip/). |

### ملاحظات

**Learn more:**

* [Supported Document Formats](https://docs.groupdocs.com/display/parsernet/Supported+Document+Formats)
* [Get supported file formats](https://docs.groupdocs.com/display/parsernet/Get+supported+file+formats)
* [Get document info](https://docs.groupdocs.com/display/parsernet/Get+document+info)

### انظر أيضًا

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

---
title: PageImageArea
second_title: GroupDocs.Parser لمرجع .NET API
description: يمثل منطقة صورة الصفحة التي تُستخدم لتمثيل صورة على الصفحة في التحليل بواسطة وظيفة القالب أو مرفق صورة إذا تم استخراج الصور من رسائل البريد الإلكتروني أو أرشيفات مضغوطة .
type: docs
weight: 110
url: /ar/net/groupdocs.parser.data/pageimagearea/
---
## PageImageArea class

يمثل منطقة صورة الصفحة التي تُستخدم لتمثيل صورة على الصفحة في التحليل بواسطة وظيفة القالب أو مرفق صورة إذا تم استخراج الصور من رسائل البريد الإلكتروني أو أرشيفات مضغوطة .

```csharp
public sealed class PageImageArea : PageArea
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [PageImageArea](pageimagearea#constructor)(Stream, FileType, double) | يقوم بتهيئة مثيل جديد لملف[`PageImageArea`](../pageimagearea) فئة . |
| [PageImageArea](pageimagearea#constructor_1)(Stream, FileType, double, Page, Rectangle) | يقوم بتهيئة مثيل جديد لملف[`PageImageArea`](../pageimagearea) فئة . |

## الخصائص

| اسم | وصف |
| --- | --- |
| [FileType](../../groupdocs.parser.data/pageimagearea/filetype) { get; } | يحصل على تنسيق الصورة. |
| [Page](../../groupdocs.parser.data/pagearea/page) { get; } | الحصول على معلومات صفحة المستند مثل فهرس الصفحة وحجم الصفحة. |
| [Rectangle](../../groupdocs.parser.data/pagearea/rectangle) { get; } | يحصل على المنطقة المستطيلة . |
| [Rotation](../../groupdocs.parser.data/pageimagearea/rotation) { get; } | يحصل على زاوية دوران الصورة. |

## طُرق

| اسم | وصف |
| --- | --- |
| [GetImageStream](../../groupdocs.parser.data/pageimagearea/getimagestream#getimagestream)() | إرجاع دفق الصورة. |
| [GetImageStream](../../groupdocs.parser.data/pageimagearea/getimagestream#getimagestream_1)(ImageOptions) | إرجاع دفق الصورة بتنسيق مختلف. |
| [Save](../../groupdocs.parser.data/pageimagearea/save#save)(string) | يحفظ الصورة في الملف . |
| [Save](../../groupdocs.parser.data/pageimagearea/save#save_1)(string, ImageOptions) | يحفظ الصورة في الملف بتنسيق مختلف. |

### ملاحظات

مثال على[`PageImageArea`](../pageimagearea) يتم استخدام الفئة كقيمة إرجاع للطرق التالية:

* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetImages`](../../groupdocs.parser/parser/getimages)

انظر الى أمثلة الاستخدام هناك.

### أنظر أيضا

* class [PageArea](../pagearea)
* مساحة الاسم [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* المجسم [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

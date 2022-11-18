---
title: GetImages
second_title: GroupDocs.Parser لمرجع .NET API
description: استخراج الصور من المستند.
type: docs
weight: 110
url: /ar/net/groupdocs.parser/parser/getimages/
---
## GetImages() {#getimages}

استخراج الصور من المستند.

```csharp
public IEnumerable<PageImageArea> GetImages()
```

### قيمة الإرجاع

مجموعة من[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) كائنات ؛ `لا شيء` إذا كان استخراج الصور غير مدعوم.

### ملاحظات

**يتعلم أكثر:**

* [استخراج الصور من المستندات](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [استخراج الصور إلى الملفات](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [استخراج الصور من مستندات Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [استخراج الصور من جداول بيانات Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [استخراج الصور من عروض Microsoft Office PowerPoint التقديمية](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [استخراج الصور من رسائل البريد الإلكتروني](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [استخراج الصور من مستندات PDF](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### أمثلة

يوضح المثال التالي كيفية استخراج جميع الصور من المستند بأكمله:

```csharp
// إنشاء مثيل لفئة المحلل اللغوي
using (Parser parser = new Parser(filePath))
{
    // استخراج الصور
    IEnumerable<PageImageArea> images = parser.GetImages();
    // تحقق مما إذا كان استخراج الصور مدعومًا
    if (images == null)
    {
        Console.WriteLine("Images extraction isn't supported");
        return;
    }
    // تكرار على الصور
    foreach (PageImageArea image in images)
    {
        // طباعة فهرس الصفحة والمستطيل ونوع الصورة:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### أنظر أيضا

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

---

## GetImages(PageAreaOptions) {#getimages_1}

استخراج الصور من المستند باستخدام خيارات التخصيص (لتعيين المنطقة المستطيلة التي تحتوي على الصور) .

```csharp
public IEnumerable<PageImageArea> GetImages(PageAreaOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| options | PageAreaOptions | خيارات استخراج الصور. |

### قيمة الإرجاع

مجموعة من[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) كائنات ؛ `لا شيء` إذا كان استخراج الصور غير مدعوم.

### ملاحظات

**يتعلم أكثر:**

* [استخراج الصور من المستندات](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [استخراج الصور إلى الملفات](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [استخراج الصور من وثيقة منطقة الصفحة](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [استخراج الصور من مستندات Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [استخراج الصور من جداول بيانات Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [استخراج الصور من عروض Microsoft Office PowerPoint التقديمية](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [استخراج الصور من رسائل البريد الإلكتروني](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [استخراج الصور من مستندات PDF](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### أمثلة

يوضح المثال التالي كيفية استخراج الصور فقط من الفناء العلوي الأيسر:

```csharp
// إنشاء مثيل لفئة المحلل اللغوي
using (Parser parser = new Parser(filePath))
{
    // إنشاء الخيارات المستخدمة لاستخراج الصور
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(0, 0), new Size(300, 100)));
    // استخراج الصور من الفناء العلوي الأيسر للصفحة:
    IEnumerable<PageImageArea> images = parser.GetImages(options);
    // تحقق مما إذا كان استخراج الصور مدعومًا
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }
    // تكرار على الصور
    foreach (PageImageArea image in images)
    {
        // طباعة فهرس الصفحة والمستطيل ونوع الصورة:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### أنظر أيضا

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

---

## GetImages(int) {#getimages_2}

استخراج الصور من صفحة المستند.

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pageIndex | Int32 | فهرس الصفحات الصفري. |

### قيمة الإرجاع

مجموعة من[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) كائنات ؛ `لا شيء` إذا كان استخراج الصور غير مدعوم.

### ملاحظات

**يتعلم أكثر:**

* [استخراج الصور من المستندات](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [استخراج الصور إلى الملفات](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [استخراج الصور من صفحة الوثيقة](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [استخراج الصور من مستندات Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [استخراج الصور من جداول بيانات Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [استخراج الصور من عروض Microsoft Office PowerPoint التقديمية](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [استخراج الصور من رسائل البريد الإلكتروني](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [استخراج الصور من مستندات PDF](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### أمثلة

لاستخراج الصور من صفحة الوثيقة ، يتم استخدام الطريقة التالية:

```csharp
// إنشاء مثيل لفئة المحلل اللغوي
using (Parser parser = new Parser(filePath))
{
    // تحقق مما إذا كان المستند يدعم استخراج الصور
    if (!parser.Features.Images)
    {
        Console.WriteLine("Document isn't supports images extraction.");
        return;
    }
    
    // احصل على معلومات المستند
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // تحقق مما إذا كان المستند يحتوي على صفحات
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // تكرار عبر الصفحات
    for (int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // طباعة رقم الصفحة 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // تكرار على الصور
        // نتجاهل التحقق من القيم الخالية لأننا تحققنا من دعم ميزة استخراج الصور مسبقًا
        foreach (PageImageArea image in parser.GetImages(pageIndex))
        {
            // طباعة مستطيل ونوع الصورة
            Console.WriteLine(string.Format("R: {0}, Text: {1}", image.Rectangle, image.FileType));
        }
    }
}
```

### أنظر أيضا

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

---

## GetImages(int, PageAreaOptions) {#getimages_3}

استخراج الصور من صفحة المستند باستخدام خيارات التخصيص (لتعيين المنطقة المستطيلة التي تحتوي على الصور) .

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex, PageAreaOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pageIndex | Int32 | فهرس الصفحات الصفري. |
| options | PageAreaOptions | خيارات استخراج الصور. |

### قيمة الإرجاع

مجموعة من[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) كائنات ؛ `لا شيء` إذا كان استخراج الصور غير مدعوم.

### ملاحظات

**يتعلم أكثر:**

* [استخراج الصور من المستندات](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [استخراج الصور إلى الملفات](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [استخراج الصور من صفحة الوثيقة](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [استخراج الصور من وثيقة منطقة الصفحة](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [استخراج الصور من مستندات Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [استخراج الصور من جداول بيانات Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [استخراج الصور من عروض Microsoft Office PowerPoint التقديمية](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [استخراج الصور من رسائل البريد الإلكتروني](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [استخراج الصور من مستندات PDF](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### أنظر أيضا

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

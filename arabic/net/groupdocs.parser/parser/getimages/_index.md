---
title: "GetImages"
second_title: "GroupDocs.Parser لـ .NET API مرجع"
description: "يستخرج الصور من المستند."
type: docs
weight: 130
url: /ar/net/groupdocs.parser/parser/getimages/
---

## GetImages() {#getimages}

يستخرج الصور من المستند.

```csharp
public IEnumerable<PageImageArea> GetImages()
```

### قيمة الإرجاع

مجموعة من كائنات [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea)؛ `null` إذا لم يكن استخراج الصور مدعومًا.

### ملاحظات

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### أمثلة

المثال التالي يوضح كيفية استخراج جميع الصور من المستند بالكامل:

```csharp
// إنشاء مثال من فئة Parser
using (Parser parser = new Parser(filePath))
{
    // استخراج الصور
    IEnumerable<PageImageArea> images = parser.GetImages();
    // التحقق مما إذا كان استخراج الصور مدعومًا
    if (images == null)
    {
        Console.WriteLine("Images extraction isn't supported");
        return;
    }
    // التكرار عبر الصور
    foreach (PageImageArea image in images)
    {
        // طباعة فهرس الصفحة، المستطيل ونوع الصورة:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### انظر أيضًا

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(PageAreaOptions) {#getimages_1}

يستخرج الصور من المستند باستخدام خيارات التخصيص (لتحديد المنطقة المستطيلة التي تحتوي على الصور).

```csharp
public IEnumerable<PageImageArea> GetImages(PageAreaOptions options)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| options | PageAreaOptions | الخيارات لاستخراج الصور. |

### قيمة الإرجاع

مجموعة من كائنات [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea)؛ `null` إذا لم يكن استخراج الصور مدعومًا.

### ملاحظات

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page area](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### أمثلة

المثال التالي يوضح كيفية استخراج الصور فقط من الزاوية العلوية اليسرى:

```csharp
// إنشاء مثال من فئة Parser
using (Parser parser = new Parser(filePath))
{
    // إنشاء الخيارات المستخدمة لاستخراج الصور
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(0, 0), new Size(300, 100)));
    // استخراج الصور من الزاوية العلوية اليسرى للصفحة:
    IEnumerable<PageImageArea> images = parser.GetImages(options);
    // التحقق مما إذا كان استخراج الصور مدعومًا
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }
    // التكرار عبر الصور
    foreach (PageImageArea image in images)
    {
        // طباعة فهرس الصفحة، المستطيل ونوع الصورة:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### انظر أيضًا

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(int) {#getimages_2}

يستخرج الصور من صفحة المستند.

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| pageIndex | Int32 | فهرس الصفحة يبدأ من الصفر. |

### قيمة الإرجاع

مجموعة من كائنات [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea)؛ `null` إذا لم يكن استخراج الصور مدعومًا.

### ملاحظات

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### أمثلة

لاستخراج الصور من صفحة مستند يتم استخدام الطريقة التالية:

```csharp
// إنشاء مثال من فئة Parser
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
    
    // التكرار عبر الصفحات
    for (int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // طباعة رقم الصفحة 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // التكرار عبر الصور
        // نتجاهل فحص القيم الفارغة لأننا تحققنا مسبقًا من دعم ميزة استخراج الصور
        foreach (PageImageArea image in parser.GetImages(pageIndex))
        {
            // اطبع مستطيلًا ونوع الصورة
            Console.WriteLine(string.Format("R: {0}, Text: {1}", image.Rectangle, image.FileType));
        }
    }
}
```

### انظر أيضًا

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(int, PageAreaOptions) {#getimages_3}

يستخرج الصور من صفحة المستند باستخدام خيارات التخصيص (لتحديد المنطقة المستطيلة التي تحتوي على الصور).

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex, PageAreaOptions options)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| pageIndex | Int32 | فهرس الصفحة يبدأ من الصفر. |
| options | PageAreaOptions | الخيارات لاستخراج الصور. |

### قيمة الإرجاع

مجموعة من كائنات [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea)؛ `null` إذا لم يكن استخراج الصور مدعومًا.

### ملاحظات

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extract images from document page area](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### انظر أيضًا

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

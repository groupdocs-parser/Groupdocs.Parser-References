---
title: "GetHyperlinks"
second_title: "GroupDocs.Parser لـ .NET API مرجع"
description: "يستخرج الروابط التشعبية من المستند."
type: docs
weight: 120
url: /ar/net/groupdocs.parser/parser/gethyperlinks/
---

## GetHyperlinks() {#gethyperlinks}

يستخرج الروابط التشعبية من المستند.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks()
```

### قيمة الإرجاع

مجموعة من كائنات [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea); `null` إذا لم يكن استخراج الروابط مدعومًا.

### أمثلة

المثال التالي يوضح كيفية استخراج جميع الروابط من المستند بالكامل:

```csharp
// إنشاء مثال من فئة Parser
using (Parser parser = new Parser(filePath))
{
    // تحقق مما إذا كان المستند يدعم استخراج الروابط
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // استخراج الروابط من المستند
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks();
    // التكرار عبر الروابط
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // طباعة نص الرابط
        Console.WriteLine(h.Text);
        // طباعة عنوان URL للرابط
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### انظر أيضًا

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int) {#gethyperlinks_2}

يستخرج الروابط التشعبية من صفحة المستند.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| pageIndex | Int32 | فهرس الصفحة يبدأ من الصفر. |

### قيمة الإرجاع

مجموعة من كائنات [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea); `null` إذا لم يكن استخراج الروابط مدعومًا.

### أمثلة

المثال التالي يوضح كيفية استخراج الروابط من صفحة المستند:

```csharp
// إنشاء مثال من فئة Parser
using (Parser parser = new Parser(filePath))
{
    // تحقق مما إذا كان المستند يدعم استخراج الروابط
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
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
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // طباعة رقم الصفحة 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // استخراج الروابط من صفحة المستند
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex);
        // التكرار عبر الروابط
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // طباعة نص الرابط
            Console.WriteLine(h.Text);
            // طباعة عنوان URL للرابط
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
    }
}
```

### انظر أيضًا

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(PageAreaOptions) {#gethyperlinks_1}

يستخرج الروابط التشعبية من المستند باستخدام خيارات التخصيص (لتحديد المنطقة المستطيلة التي تحتوي على الروابط التشعبية).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(PageAreaOptions options)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| options | PageAreaOptions | الخيارات لاستخراج الروابط. |

### قيمة الإرجاع

مجموعة من كائنات [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea); `null` إذا لم يكن استخراج الروابط مدعومًا.

### أمثلة

المثال التالي يوضح كيفية استخراج الروابط من منطقة صفحة المستند:

```csharp
// إنشاء مثال من فئة Parser
using (Parser parser = new Parser(filePath))
{
    // تحقق مما إذا كان المستند يدعم استخراج الروابط
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // إنشاء الخيارات المستخدمة لاستخراج الروابط
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // استخراج الروابط من منطقة صفحة المستند
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(options);
    // التكرار عبر الروابط
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // طباعة نص الرابط
        Console.WriteLine(h.Text);
        // طباعة عنوان URL للرابط
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### انظر أيضًا

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int, PageAreaOptions) {#gethyperlinks_3}

يستخرج الروابط التشعبية من صفحة المستند باستخدام خيارات التخصيص (لتحديد المنطقة المستطيلة التي تحتوي على الروابط التشعبية).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex, PageAreaOptions options)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| pageIndex | Int32 | فهرس الصفحة يبدأ من الصفر. |
| options | PageAreaOptions | الخيارات لاستخراج الروابط. |

### قيمة الإرجاع

مجموعة من كائنات [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea); `null` إذا لم يكن استخراج الروابط مدعومًا.

### أمثلة

المثال التالي يوضح كيفية استخراج الروابط التشعبية من منطقة صفحة المستند باستخدام خيارات التخصيص:

```csharp
// إنشاء مثال من فئة Parser
using (Parser parser = new Parser(filePath))
{
    // تحقق مما إذا كان المستند يدعم استخراج الروابط
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
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
    
    // إنشاء الخيارات المستخدمة لاستخراج الروابط
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // التكرار عبر الصفحات
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // طباعة رقم الصفحة 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));         
        // استخراج الروابط من منطقة صفحة المستند
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex, options);
        // التكرار عبر الروابط
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // طباعة نص الرابط
            Console.WriteLine(h.Text);
            // طباعة عنوان URL للرابط
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
}
```

### انظر أيضًا

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

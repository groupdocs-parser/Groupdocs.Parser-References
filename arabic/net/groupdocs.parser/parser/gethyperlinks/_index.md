---
title: GetHyperlinks
second_title: GroupDocs.Parser لمرجع .NET API
description: استخراج الارتباطات التشعبية من المستند.
type: docs
weight: 100
url: /ar/net/groupdocs.parser/parser/gethyperlinks/
---
## GetHyperlinks() {#gethyperlinks}

استخراج الارتباطات التشعبية من المستند.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks()
```

### قيمة الإرجاع

مجموعة من[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) كائنات ؛ `لا شيء` إذا كان استخراج الارتباطات التشعبية غير مدعوم.

### أمثلة

يوضح المثال التالي كيفية استخراج كافة الارتباطات التشعبية من المستند بأكمله:

```csharp
// إنشاء مثيل لفئة المحلل اللغوي
using (Parser parser = new Parser(filePath))
{
    // تحقق مما إذا كان المستند يدعم استخراج الارتباط التشعبي
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // استخراج الارتباطات التشعبية من المستند
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks();
    // كرر عبر الارتباطات التشعبية
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // طباعة نص الارتباط التشعبي
        Console.WriteLine(h.Text);
        // طباعة عنوان URL للارتباط التشعبي
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### أنظر أيضا

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int) {#gethyperlinks_2}

استخراج الارتباطات التشعبية من صفحة المستند.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pageIndex | Int32 | فهرس الصفحات الصفري. |

### قيمة الإرجاع

مجموعة من[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) كائنات ؛ `لا شيء` إذا كان استخراج الارتباطات التشعبية غير مدعوم.

### أمثلة

يوضح المثال التالي كيفية استخراج الارتباطات التشعبية من صفحة المستند:

```csharp
// إنشاء مثيل لفئة المحلل اللغوي
using (Parser parser = new Parser(filePath))
{
    // تحقق مما إذا كان المستند يدعم استخراج الارتباط التشعبي
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
    // تكرار عبر الصفحات
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // طباعة رقم الصفحة 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // استخراج الارتباطات التشعبية من صفحة المستند
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex);
        // كرر عبر الارتباطات التشعبية
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // طباعة نص الارتباط التشعبي
            Console.WriteLine(h.Text);
            // طباعة عنوان URL للارتباط التشعبي
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
    }
}
```

### أنظر أيضا

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

---

## GetHyperlinks(PageAreaOptions) {#gethyperlinks_1}

استخراج الارتباطات التشعبية من المستند باستخدام خيارات التخصيص (لتعيين المنطقة المستطيلة التي تحتوي على ارتباطات تشعبية) .

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(PageAreaOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| options | PageAreaOptions | خيارات استخراج الارتباطات التشعبية. |

### قيمة الإرجاع

مجموعة من[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) كائنات ؛ `لا شيء` إذا كان استخراج الارتباطات التشعبية غير مدعوم.

### أمثلة

يوضح المثال التالي كيفية استخراج الارتباطات التشعبية من منطقة صفحة المستند:

```csharp
// إنشاء مثيل لفئة المحلل اللغوي
using (Parser parser = new Parser(filePath))
{
    // تحقق مما إذا كان المستند يدعم استخراج الارتباط التشعبي
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // إنشاء الخيارات المستخدمة لاستخراج الارتباط التشعبي
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // استخراج الارتباطات التشعبية من منطقة صفحة المستند
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(options);
    // كرر عبر الارتباطات التشعبية
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // طباعة نص الارتباط التشعبي
        Console.WriteLine(h.Text);
        // طباعة عنوان URL للارتباط التشعبي
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### أنظر أيضا

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int, PageAreaOptions) {#gethyperlinks_3}

استخراج الارتباطات التشعبية من صفحة المستند باستخدام خيارات التخصيص (لتعيين المنطقة المستطيلة التي تحتوي على ارتباطات تشعبية) .

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex, PageAreaOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pageIndex | Int32 | فهرس الصفحات الصفري. |
| options | PageAreaOptions | خيارات استخراج الارتباطات التشعبية. |

### قيمة الإرجاع

مجموعة من[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) كائنات ؛ `لا شيء` إذا كان استخراج الارتباطات التشعبية غير مدعوم.

### أمثلة

يوضح المثال التالي كيفية استخراج الارتباطات التشعبية من منطقة صفحة المستند باستخدام خيارات التخصيص:

```csharp
// إنشاء مثيل لفئة المحلل اللغوي
using (Parser parser = new Parser(filePath))
{
    // تحقق مما إذا كان المستند يدعم استخراج الارتباط التشعبي
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
    
    // إنشاء الخيارات المستخدمة لاستخراج الارتباط التشعبي
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // تكرار عبر الصفحات
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // طباعة رقم الصفحة 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));         
        // استخراج الارتباطات التشعبية من منطقة صفحة المستند
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex, options);
        // كرر عبر الارتباطات التشعبية
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // طباعة نص الارتباط التشعبي
            Console.WriteLine(h.Text);
            // طباعة عنوان URL للارتباط التشعبي
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
}
```

### أنظر أيضا

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

---
title: GetTables
second_title: GroupDocs.Parser لمرجع .NET API
description: استخراج الجداول من المستند.
type: docs
weight: 140
url: /ar/net/groupdocs.parser/parser/gettables/
---
## GetTables(PageTableAreaOptions) {#gettables}

استخراج الجداول من المستند.

```csharp
public IEnumerable<PageTableArea> GetTables(PageTableAreaOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| options | PageTableAreaOptions | خيارات استخراج الجداول. |

### قيمة الإرجاع

مجموعة من[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) كائنات ؛ `باطل` إذا كان استخراج الجداول غير مدعوم.

### أمثلة

يوضح المثال التالي كيفية استخراج الجداول من المستند بأكمله:

```csharp
// إنشاء مثيل لفئة المحلل اللغوي
using (Parser parser = new Parser(filePath))
{
    // تحقق مما إذا كان المستند يدعم استخراج الجدول
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // إنشاء تخطيط الجداول
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // إنشاء خيارات لاستخراج الجدول
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // استخراج الجداول من الوثيقة
    IEnumerable<PageTableArea> tables = parser.GetTables(options);
    // تكرار على الطاولات
    foreach (PageTableArea t in tables)
    {
        // كرر على الصفوف
        for (int row = 0; row < t.RowCount; row++)
        {
            // التكرار على الأعمدة
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // احصل على خلية الجدول
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // طباعة نص خلية الجدول
                    Console.Write(cell.Text);
                    Console.Write(" | ");
                }
            }
            Console.WriteLine();
        }
        Console.WriteLine();
    }
}
```

### أنظر أيضا

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

---

## GetTables(int, PageTableAreaOptions) {#gettables_1}

استخراج الجداول من صفحة المستند.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex, PageTableAreaOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pageIndex | Int32 | فهرس الصفحات الصفري. |
| options | PageTableAreaOptions | خيارات استخراج الجداول. |

### قيمة الإرجاع

مجموعة من[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) كائنات ؛ `باطل` إذا كان استخراج الجداول غير مدعوم.

### أمثلة

يوضح المثال التالي كيفية استخراج الجداول من صفحة المستند:

```csharp
// إنشاء مثيل لفئة المحلل اللغوي
using (Parser parser = new Parser(filePath))
{
    // تحقق مما إذا كان المستند يدعم استخراج الجدول
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // إنشاء تخطيط الجداول
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // إنشاء خيارات لاستخراج الجدول
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
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
        // استخراج الجداول من صفحة الوثيقة
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex, options);
        // تكرار على الطاولات
        foreach (PageTableArea t in tables)
        {
            // كرر على الصفوف
            for (int row = 0; row < t.RowCount; row++)
            {
                // التكرار على الأعمدة
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // احصل على خلية الجدول
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // طباعة نص خلية الجدول
                        Console.Write(cell.Text);
                        Console.Write(" | ");
                    }
                }
                Console.WriteLine();
            }
            Console.WriteLine();
        }
    }
}
```

### أنظر أيضا

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

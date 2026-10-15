---
title: "GetTables"
second_title: "GroupDocs.Parser لـ .NET API مرجع"
description: "يستخرج الجداول من المستند."
type: docs
weight: 170
url: /ar/net/groupdocs.parser/parser/gettables/
---

## GetTables(PageTableAreaOptions) {#gettables_1}

يستخرج الجداول من المستند.

```csharp
public IEnumerable<PageTableArea> GetTables(PageTableAreaOptions options)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| options | PageTableAreaOptions | الخيارات لاستخراج الجداول. |

### قيمة الإرجاع

مجموعة من كائنات [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea)؛ `null` إذا لم يكن استخراج الجداول مدعومًا.

### أمثلة

المثال التالي يوضح كيفية استخراج الجداول من المستند بالكامل:

```csharp
// إنشاء مثال من فئة Parser
using (Parser parser = new Parser(filePath))
{
    // تحقق مما إذا كان المستند يدعم استخراج الجداول
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // إنشاء تخطيط الجداول
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // إنشاء الخيارات لاستخراج الجداول
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // استخراج الجداول من المستند
    IEnumerable<PageTableArea> tables = parser.GetTables(options);
    // التكرار عبر الجداول
    foreach (PageTableArea t in tables)
    {
        // التكرار عبر الصفوف
        for (int row = 0; row < t.RowCount; row++)
        {
            // التكرار عبر الأعمدة
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // الحصول على خلية الجدول
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

### انظر أيضًا

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables(int, PageTableAreaOptions) {#gettables_3}

يستخرج الجداول من صفحة المستند.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex, PageTableAreaOptions options)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| pageIndex | Int32 | فهرس الصفحة يبدأ من الصفر. |
| options | PageTableAreaOptions | الخيارات لاستخراج الجداول. |

### قيمة الإرجاع

مجموعة من كائنات [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea)؛ `null` إذا لم يكن استخراج الجداول مدعومًا.

### أمثلة

المثال التالي يوضح كيفية استخراج الجداول من صفحة المستند:

```csharp
// إنشاء مثال من فئة Parser
using (Parser parser = new Parser(filePath))
{
    // تحقق مما إذا كان المستند يدعم استخراج الجداول
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // إنشاء تخطيط الجداول
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // إنشاء الخيارات لاستخراج الجداول
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // احصل على معلومات المستند
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // تحقق مما إذا كان المستند يحتوي على صفحات
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("The document has no pages.");
        return;
    }
    // التكرار عبر الصفحات
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // طباعة رقم الصفحة 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // استخراج الجداول من صفحة المستند
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex, options);
        // التكرار عبر الجداول
        foreach (PageTableArea t in tables)
        {
            // التكرار عبر الصفوف
            for (int row = 0; row < t.RowCount; row++)
            {
                // التكرار عبر الأعمدة
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // الحصول على خلية الجدول
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

### انظر أيضًا

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables() {#gettables}

يستخرج الجداول من المستند.

```csharp
public IEnumerable<PageTableArea> GetTables()
```

### قيمة الإرجاع

مجموعة من كائنات [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea)؛ `null` إذا لم يكن استخراج الجداول مدعومًا.

### أمثلة

المثال التالي يوضح كيفية استخراج الجداول من المستند بالكامل:

```csharp
// إنشاء مثال من فئة Parser
using (Parser parser = new Parser(filePath))
{
    // تحقق مما إذا كان المستند يدعم استخراج الجداول
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // استخراج الجداول من المستند
    IEnumerable<PageTableArea> tables = parser.GetTables();
    // التكرار عبر الجداول
    foreach (PageTableArea t in tables)
    {
        // التكرار عبر الصفوف
        for (int row = 0; row < t.RowCount; row++)
        {
            // التكرار عبر الأعمدة
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // الحصول على خلية الجدول
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

### انظر أيضًا

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables(int) {#gettables_2}

يستخرج الجداول من صفحة المستند.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| pageIndex | Int32 | فهرس الصفحة يبدأ من الصفر. |

### قيمة الإرجاع

مجموعة من كائنات [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea)؛ `null` إذا لم يكن استخراج الجداول مدعومًا.

### أمثلة

المثال التالي يوضح كيفية استخراج الجداول من صفحة المستند:

```csharp
// إنشاء مثال من فئة Parser
using (Parser parser = new Parser(filePath))
{
    // تحقق مما إذا كان المستند يدعم استخراج الجداول
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // احصل على معلومات المستند
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // تحقق مما إذا كان المستند يحتوي على صفحات
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("The document has no pages.");
        return;
    }
    // التكرار عبر الصفحات
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // طباعة رقم الصفحة 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // استخراج الجداول من صفحة المستند
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex);
        // التكرار عبر الجداول
        foreach (PageTableArea t in tables)
        {
            // التكرار عبر الصفوف
            for (int row = 0; row < t.RowCount; row++)
            {
                // التكرار عبر الأعمدة
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // الحصول على خلية الجدول
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

### انظر أيضًا

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

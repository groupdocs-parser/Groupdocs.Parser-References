---
title: ExtractText
second_title: GroupDocs.Parser لمرجع .NET API
description: لاستخراج نص من المستندTocItemgroupdocs.parser.data/tocitem يشير الكائن .
type: docs
weight: 50
url: /ar/net/groupdocs.parser.data/tocitem/extracttext/
---
## TocItem.ExtractText method

لاستخراج نص من المستند[`TocItem`](../../tocitem) يشير الكائن .

```csharp
public virtual TextReader ExtractText()
```

### قيمة الإرجاع

مثال علىTextReader فئة مع النص المستخرج.

### أمثلة

المثال التالي كيفية استخراج نص حسب عنصر جدول المحتويات:

```csharp
// إنشاء مثيل لفئة المحلل اللغوي
using (Parser parser = new Parser(Constants.SampleDocxWithToc))
{
    // احصل على جدول المحتويات
    IEnumerable<TocItem> tocItems = parser.GetToc();
    // تحقق مما إذا كان استخراج toc مدعومًا
    if (tocItems == null)
    {
        Console.WriteLine("Table of contents extraction isn't supported");
    }
    // كرر على العناصر
    foreach (TocItem tocItem in tocItems)
    {
        // اطبع نص الفصل
        using (TextReader reader = tocItem.ExtractText())
        {
            Console.WriteLine("----");
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### أنظر أيضا

* class [TocItem](../../tocitem)
* مساحة الاسم [GroupDocs.Parser.Data](../../tocitem)
* المجسم [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

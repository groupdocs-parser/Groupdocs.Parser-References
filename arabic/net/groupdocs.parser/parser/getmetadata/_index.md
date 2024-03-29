---
title: GetMetadata
second_title: GroupDocs.Parser لمرجع .NET API
description: استخراج البيانات الوصفية من المستند.
type: docs
weight: 120
url: /ar/net/groupdocs.parser/parser/getmetadata/
---
## Parser.GetMetadata method

استخراج البيانات الوصفية من المستند.

```csharp
public IEnumerable<MetadataItem> GetMetadata()
```

### قيمة الإرجاع

مجموعة من عناصر البيانات الوصفية ؛ `باطل` إذا كان استخراج البيانات الوصفية غير مدعوم.

### ملاحظات

**يتعلم أكثر:**

* [استخراج البيانات الوصفية من الوثائق](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+documents)
* [استخراج البيانات الوصفية من مستندات Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+Word+documents)
* [استخراج البيانات الوصفية من جداول بيانات Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+Excel+spreadsheets)
* [استخراج البيانات الوصفية من عروض Microsoft Office PowerPoint التقديمية](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+PowerPoint+presentations)
* [استخراج البيانات الوصفية من مستندات PDF](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+PDF+documents)
* [استخراج البيانات الوصفية من رسائل البريد الإلكتروني](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Emails)

### أمثلة

يوضح المثال التالي كيفية استخراج البيانات الأولية من مستند:

```csharp
// إنشاء مثيل لفئة المحلل اللغوي
using(Parser parser = new Parser(filePath))
{
    // استخراج البيانات الوصفية من الوثيقة
    IEnumerable<MetadataItem> metadata = parser.GetMetadata();
    // تحقق مما إذا كان استخراج البيانات الوصفية مدعومًا
    if(metadata == null)
    {
        Console.WriteLine("Metatada extraction isn't supported");
    }
 
    // كرر عبر عناصر البيانات الوصفية
    foreach(MetadataItem item in metadata)
    {
        // طباعة اسم العنصر وقيمته
        Console.WriteLine(string.Format("{0}: {1}", item.Name, item.Value));
    }
}
```

### أنظر أيضا

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

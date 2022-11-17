---
title: GetText
second_title: GroupDocs.Parser لمرجع .NET API
description: استخراج نص من المستند.
type: docs
weight: 150
url: /ar/net/groupdocs.parser/parser/gettext/
---
## GetText() {#gettext}

استخراج نص من المستند.

```csharp
public TextReader GetText()
```

### قيمة الإرجاع

مثيلTextReader فئة مع النص المستخرج `لا شيء` إذا كان استخراج النص غير مدعوم.

### ملاحظات

**يتعلم أكثر:**

* [استخراج النص من المستندات](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [استخراج النص في الوضع الدقيق](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### أمثلة

يوضح المثال التالي كيفية استخراج نص من مستند:

```csharp
// إنشاء مثيل لفئة المحلل اللغوي
using(Parser parser = new Parser(filePath))
{
    // استخراج نص في القارئ
    using(TextReader reader = parser.GetText())
    {
        // طباعة نص من المستند
        // إذا لم يكن استخراج النص مدعومًا ، يكون القارئ فارغًا
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### أنظر أيضا

* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

---

## GetText(TextOptions) {#gettext_1}

استخراج صفحة نصية من المستند باستخدام خيارات النص (لتمكين وضع الاستخراج السريع للنص الخام) .

```csharp
public TextReader GetText(TextOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| options | TextOptions | خيارات استخراج النص. |

### قيمة الإرجاع

مثيلTextReader فئة مع النص المستخرج `لا شيء` إذا كان استخراج النص غير مدعوم.

### ملاحظات

**يتعلم أكثر:**

* [استخراج النص في الوضع الدقيق](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [استخراج النص في صيغة Raw](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### أمثلة

يوضح المثال التالي كيفية استخراج نص خام من مستند:

```csharp
// إنشاء مثيل لفئة المحلل اللغوي
using(Parser parser = new Parser(filePath))
{
    // استخراج نص خام في القارئ
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // طباعة نص من المستند
        // إذا لم يكن استخراج النص مدعومًا ، يكون القارئ فارغًا
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### أنظر أيضا

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

استخراج نص من صفحة المستند.

```csharp
public TextReader GetText(int pageIndex)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pageIndex | Int32 | فهرس الصفحات الصفري. |

### قيمة الإرجاع

مثيلTextReader فئة مع النص المستخرج `لا شيء` إذا لم يتم دعم استخراج صفحة النص.

### ملاحظات

**يتعلم أكثر:**

* [استخراج النص في الوضع الدقيق](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### أمثلة

يوضح المثال التالي كيفية استخراج نص من صفحة المستند:

```csharp
// إنشاء مثيل لفئة المحلل اللغوي
using(Parser parser = new Parser(filePath))
{
    // تحقق مما إذا كان المستند يدعم استخراج النص
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // احصل على معلومات المستند
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // تحقق مما إذا كان المستند يحتوي على صفحات
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // تكرار عبر الصفحات
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // طباعة رقم الصفحة 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // استخراج نص في القارئ
        using(TextReader reader = parser.GetText(p))
        {
            // طباعة نص من المستند
            // نتجاهل التحقق من القيم الخالية لأننا تحققنا من دعم ميزة استخراج النص مسبقًا
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### أنظر أيضا

* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

---

## GetText(int, TextOptions) {#gettext_3}

استخراج نص من صفحة المستند باستخدام خيارات النص (لتمكين وضع الاستخراج السريع للنص الخام) .

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pageIndex | Int32 | فهرس الصفحات الصفري. |
| options | TextOptions | خيارات استخراج النص. |

### قيمة الإرجاع

مثيلTextReader فئة مع النص المستخرج `لا شيء` إذا لم يتم دعم استخراج صفحة النص.

### ملاحظات

**يتعلم أكثر:**

* [استخراج النص في الوضع الدقيق](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [استخراج النص في صيغة Raw](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### أمثلة

يوضح المثال التالي كيفية استخراج نص خام من صفحة المستند:

```csharp
// إنشاء مثيل لفئة المحلل اللغوي
using(Parser parser = new Parser(filePath))
{
    // تحقق مما إذا كان المستند يدعم استخراج النص
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // احصل على معلومات المستند
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // تحقق مما إذا كان المستند يحتوي على صفحات
    if(documentInfo == null || documentInfo.RawPageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // تكرار عبر الصفحات
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // طباعة رقم الصفحة 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // استخراج نص في القارئ
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // طباعة نص من المستند
            // نتجاهل التحقق من القيم الخالية لأننا تحققنا من دعم ميزة استخراج النص مسبقًا
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### أنظر أيضا

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

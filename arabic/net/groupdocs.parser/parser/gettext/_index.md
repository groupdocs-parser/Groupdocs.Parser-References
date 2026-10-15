---
title: "GetText"
second_title: "GroupDocs.Parser لـ .NET API مرجع"
description: "يستخرج نصًا من المستند."
type: docs
weight: 180
url: /ar/net/groupdocs.parser/parser/gettext/
---

## GetText() {#gettext}

يستخرج نصًا من المستند.

```csharp
public TextReader GetText()
```

### قيمة الإرجاع

مثال على فئة TextReader مع النص المستخرج؛ `null` إذا لم يكن استخراج النص مدعومًا.

### ملاحظات

**Learn more:**

* [Extract text from documents](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### أمثلة

المثال التالي يوضح كيفية استخراج نص من مستند:

```csharp
// إنشاء مثال من فئة Parser
using(Parser parser = new Parser(filePath))
{
    // استخراج نص إلى القارئ
    using(TextReader reader = parser.GetText())
    {
        // طباعة نص من المستند
        // إذا لم يكن استخراج النص مدعومًا، يكون القارئ null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### انظر أيضًا

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(TextOptions) {#gettext_1}

يستخرج صفحة نصية من المستند باستخدام خيارات النص (لتمكين وضع استخراج النص الخام السريع).

```csharp
public TextReader GetText(TextOptions options)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| options | TextOptions | خيارات استخراج النص. |

### قيمة الإرجاع

مثال على فئة TextReader مع النص المستخرج؛ `null` إذا لم يكن استخراج النص مدعومًا.

### ملاحظات

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### أمثلة

المثال التالي يوضح كيفية استخراج نص خام من مستند:

```csharp
// إنشاء مثال من فئة Parser
using(Parser parser = new Parser(filePath))
{
    // استخراج نص خام إلى القارئ
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // طباعة نص من المستند
        // إذا لم يكن استخراج النص مدعومًا، يكون القارئ null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### انظر أيضًا

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

يستخرج نصًا من صفحة المستند.

```csharp
public TextReader GetText(int pageIndex)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| pageIndex | Int32 | فهرس الصفحة يبدأ من الصفر. |

### قيمة الإرجاع

مثال على فئة TextReader مع النص المستخرج؛ `null` إذا لم يكن استخراج صفحة النص مدعومًا.

### ملاحظات

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### أمثلة

المثال التالي يوضح كيفية استخراج نص من صفحة المستند:

```csharp
// إنشاء مثال من فئة Parser
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
 
    // التكرار عبر الصفحات
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // طباعة رقم الصفحة 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // استخراج نص إلى القارئ
        using(TextReader reader = parser.GetText(p))
        {
            // طباعة نص من المستند
            // نتجاهل فحص null لأننا قد تحققنا مسبقًا من دعم ميزة استخراج النص
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### انظر أيضًا

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(int, TextOptions) {#gettext_3}

يستخرج نصًا من صفحة المستند باستخدام خيارات النص (لتمكين وضع استخراج النص الخام السريع).

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| pageIndex | Int32 | فهرس الصفحة يبدأ من الصفر. |
| options | TextOptions | خيارات استخراج النص. |

### قيمة الإرجاع

مثال على فئة TextReader مع النص المستخرج؛ `null` إذا لم يكن استخراج صفحة النص مدعومًا.

### ملاحظات

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### أمثلة

المثال التالي يوضح كيفية استخراج نص خام من صفحة المستند:

```csharp
// إنشاء مثال من فئة Parser
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
 
    // التكرار عبر الصفحات
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // طباعة رقم الصفحة 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // استخراج نص إلى القارئ
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // طباعة نص من المستند
            // نتجاهل فحص null لأننا قد تحققنا مسبقًا من دعم ميزة استخراج النص
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### انظر أيضًا

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

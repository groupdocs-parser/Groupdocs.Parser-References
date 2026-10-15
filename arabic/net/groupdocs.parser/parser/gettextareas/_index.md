---
title: "GetTextAreas"
second_title: "GroupDocs.Parser لـ .NET API مرجع"
description: "يستخرج مناطق النص من المستند."
type: docs
weight: 190
url: /ar/net/groupdocs.parser/parser/gettextareas/
---

## GetTextAreas() {#gettextareas}

يستخرج مناطق النص من المستند.

```csharp
public IEnumerable<PageTextArea> GetTextAreas()
```

### قيمة الإرجاع

مجموعة من كائنات [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea)؛ `null` إذا لم يكن استخراج مناطق النص مدعومًا.

### ملاحظات

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### أمثلة

المثال التالي يوضح كيفية استخراج جميع مناطق النص من المستند بالكامل:

```csharp
// إنشاء مثال من فئة Parser
using(Parser parser = new Parser(filePath))
{
    // استخراج مناطق النص
    IEnumerable<PageTextArea> areas = parser.GetTextAreas();
    // التحقق مما إذا كان استخراج مناطق النص مدعومًا
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // تكرار عبر مناطق نص الصفحة
    foreach(PageTextArea a in areas)
    {
        // طباعة فهرس الصفحة، المستطيل وقيمة منطقة النص:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### انظر أيضًا

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(PageTextAreaOptions) {#gettextareas_1}

يستخرج مناطق النص من المستند باستخدام خيارات التخصيص (التعبير النمطي، مطابقة الحالة، إلخ).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(PageTextAreaOptions options)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| options | PageTextAreaOptions | خيارات استخراج مناطق النص. |

### قيمة الإرجاع

مجموعة من كائنات [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea)؛ `null` إذا لم يكن استخراج مناطق النص مدعومًا.

### ملاحظات

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### أمثلة

المثال التالي يوضح كيفية استخراج مناطق النص التي تحتوي على أرقام فقط من الزاوية العلوية اليسرى:

```csharp
// إنشاء مثال من فئة Parser
using(Parser parser = new Parser(filePath))
{
    // إنشاء الخيارات المستخدمة لاستخراج مناطق النص
    PageTextAreaOptions options = new PageTextAreaOptions("[0-9]+", new Rectangle(new Point(0, 0), new Size(300, 100)));

    // استخراج مناطق النص التي تحتوي على أرقام فقط من الزاوية العلوية اليسرى للصفحة:
    IEnumerable<PageTextArea> areas = parser.GetTextAreas(options);
    // التحقق مما إذا كان استخراج مناطق النص مدعومًا
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // تكرار عبر مناطق نص الصفحة
    foreach(PageTextArea a in areas)
    {
        // طباعة فهرس الصفحة، المستطيل وقيمة منطقة النص:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### انظر أيضًا

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(int) {#gettextareas_2}

يستخرج مناطق النص من صفحة المستند.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| pageIndex | Int32 | فهرس الصفحة يبدأ من الصفر. |

### قيمة الإرجاع

مجموعة من كائنات [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea)؛ `null` إذا لم يكن استخراج مناطق النص مدعومًا.

### ملاحظات

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### أمثلة

لاستخراج مناطق النص من صفحة المستند يتم استخدام الطريقة التالية:

```csharp
// إنشاء مثال من فئة Parser
using(Parser parser = new Parser(filePath))
{
    // التحقق مما إذا كان المستند يدعم استخراج مناطق النص
    if(!parser.Features.TextAreas)
    {
        Console.WriteLine("Document isn't supports text areas extraction.");
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
    for(int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // طباعة رقم الصفحة 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
 
        // تكرار عبر مناطق نص الصفحة
        // نتجاهل فحص null لأننا قد تحققنا من دعم ميزة استخراج مناطق النص مسبقًا
        foreach(PageTextArea a in parser.GetTextAreas(pageIndex))
        {
            // طباعة مستطيل وقيمة منطقة النص:
            Console.WriteLine(string.Format("R: {0}, Text: {1}", a.Rectangle, a.Text));
        }
    }
}
```

### انظر أيضًا

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(int, PageTextAreaOptions) {#gettextareas_3}

يستخرج مناطق النص من صفحة المستند باستخدام خيارات التخصيص (التعبير النمطي، مطابقة الحالة، إلخ).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex, PageTextAreaOptions options)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| pageIndex | Int32 | فهرس الصفحة يبدأ من الصفر. |
| options | PageTextAreaOptions | خيارات استخراج مناطق النص. |

### قيمة الإرجاع

مجموعة من كائنات [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea)؛ `null` إذا لم يكن استخراج مناطق النص مدعومًا.

### ملاحظات

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### انظر أيضًا

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

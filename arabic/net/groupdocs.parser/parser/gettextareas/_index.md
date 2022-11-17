---
title: GetTextAreas
second_title: GroupDocs.Parser لمرجع .NET API
description: استخراج مناطق النص من المستند.
type: docs
weight: 160
url: /ar/net/groupdocs.parser/parser/gettextareas/
---
## GetTextAreas() {#gettextareas}

استخراج مناطق النص من المستند.

```csharp
public IEnumerable<PageTextArea> GetTextAreas()
```

### قيمة الإرجاع

مجموعة من[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) كائنات ؛ `لا شيء` إذا لم يتم دعم استخراج مناطق النص.

### ملاحظات

**يتعلم أكثر:**

* [استخراج مناطق النص](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### أمثلة

يوضح المثال التالي كيفية استخراج جميع مناطق النص من المستند بأكمله:

```csharp
// إنشاء مثيل لفئة المحلل اللغوي
using(Parser parser = new Parser(filePath))
{
    // استخراج مناطق النص
    IEnumerable<PageTextArea> areas = parser.GetTextAreas();
    // تحقق مما إذا كان استخراج مناطق النص مدعومًا
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // كرر عبر مناطق نص الصفحة
    foreach(PageTextArea a in areas)
    {
        // طباعة فهرس الصفحة والمستطيل وقيمة مساحة النص:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### أنظر أيضا

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

---

## GetTextAreas(PageTextAreaOptions) {#gettextareas_1}

استخراج مناطق النص من المستند باستخدام خيارات التخصيص (التعبير العادي ، حالة المطابقة ، إلخ.) .

```csharp
public IEnumerable<PageTextArea> GetTextAreas(PageTextAreaOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| options | PageTextAreaOptions | خيارات استخراج منطقة النص. |

### قيمة الإرجاع

مجموعة من[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) كائنات ؛ `لا شيء` إذا لم يتم دعم استخراج مناطق النص.

### ملاحظات

**يتعلم أكثر:**

* [استخراج مناطق النص](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### أمثلة

يوضح المثال التالي كيفية استخراج مناطق النص ذات الأرقام من الفناء العلوي الأيسر:

```csharp
// إنشاء مثيل لفئة المحلل اللغوي
using(Parser parser = new Parser(filePath))
{
    // قم بإنشاء الخيارات المستخدمة لاستخراج منطقة النص
    PageTextAreaOptions options = new PageTextAreaOptions("[0-9]+", new Rectangle(new Point(0, 0), new Size(300, 100)));

    // استخراج مناطق النص التي تحتوي على أرقام فقط من الفناء العلوي الأيسر للصفحة:
    IEnumerable<PageTextArea> areas = parser.GetTextAreas(options);
    // تحقق مما إذا كان استخراج مناطق النص مدعومًا
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // كرر عبر مناطق نص الصفحة
    foreach(PageTextArea a in areas)
    {
        // طباعة فهرس الصفحة والمستطيل وقيمة مساحة النص:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### أنظر أيضا

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

---

## GetTextAreas(int) {#gettextareas_2}

استخراج مناطق النص من صفحة المستند.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pageIndex | Int32 | فهرس الصفحات الصفري. |

### قيمة الإرجاع

مجموعة من[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) كائنات ؛ `لا شيء` إذا لم يتم دعم استخراج مناطق النص.

### ملاحظات

**يتعلم أكثر:**

* [استخراج مناطق النص](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### أمثلة

لاستخراج مناطق النص من صفحة المستند ، يتم استخدام الطريقة التالية:

```csharp
// إنشاء مثيل لفئة المحلل اللغوي
using(Parser parser = new Parser(filePath))
{
    // تحقق مما إذا كان المستند يدعم استخراج مناطق النص
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
 
    // تكرار عبر الصفحات
    for(int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // طباعة رقم الصفحة 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
 
        // كرر عبر مناطق نص الصفحة
        // نتجاهل التحقق من القيم الخالية لأننا تحققنا من دعم ميزة استخراج مناطق النص مسبقًا
        foreach(PageTextArea a in parser.GetTextAreas(pageIndex))
        {
            // طباعة مستطيل وقيمة منطقة النص:
            Console.WriteLine(string.Format("R: {0}, Text: {1}", a.Rectangle, a.Text));
        }
    }
}
```

### أنظر أيضا

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

---

## GetTextAreas(int, PageTextAreaOptions) {#gettextareas_3}

استخراج مناطق النص من صفحة المستند باستخدام خيارات التخصيص (التعبير العادي ، حالة المطابقة ، إلخ.) .

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex, PageTextAreaOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pageIndex | Int32 | فهرس الصفحات الصفري. |
| options | PageTextAreaOptions | خيارات استخراج منطقة النص. |

### قيمة الإرجاع

مجموعة من[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) كائنات ؛ `لا شيء` إذا لم يتم دعم استخراج مناطق النص.

### ملاحظات

**يتعلم أكثر:**

* [استخراج مناطق النص](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### أنظر أيضا

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

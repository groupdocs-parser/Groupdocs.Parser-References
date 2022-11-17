---
title: Search
second_title: GroupDocs.Parser لمرجع .NET API
description: عمليات البحث أkeyword في المستند.
type: docs
weight: 200
url: /ar/net/groupdocs.parser/parser/search/
---
## Search(string) {#search}

عمليات البحث أ*keyword* في المستند.

```csharp
public IEnumerable<SearchResult> Search(string keyword)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| keyword | String | الكلمة الرئيسية للبحث. |

### قيمة الإرجاع

مجموعة من[`SearchResult`](../../../groupdocs.parser.data/searchresult) أشياء؛ `لا شيء` إذا لم يتم دعم البحث.

### ملاحظات

**يتعلم أكثر:**

* [نص البحث](https://docs.groupdocs.com/display/parsernet/Search+text)
* [ابحث عن نص في مستندات Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [ابحث عن نص في جداول بيانات Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [نص البحث في عروض Microsoft Office PowerPoint التقديمية](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [ابحث عن نص في مستندات PDF](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [نص البحث في رسائل البريد الإلكتروني](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [البحث عن نص في الكتب الإلكترونية EPUB](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [نص البحث في مستندات HTML](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [ابحث عن نص في أقسام Microsoft OneNote](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### أمثلة

يوضح المثال التالي كيفية البحث عن كلمة أساسية في مستند:

```csharp
// إنشاء مثيل لفئة المحلل اللغوي
using(Parser parser = new Parser(filePath))
{
    // البحث عن كلمة أساسية:
    IEnumerable<SearchResult> sr = parser.Search("page number");
    // تحقق مما إذا كان البحث مدعومًا
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // كرر عبر نتائج البحث
    foreach(SearchResult s in sr)
    {
        // طباعة فهرس والنص الذي تم العثور عليه:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

### أنظر أيضا

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

---

## Search(string, SearchOptions) {#search_1}

عمليات البحث أ*keyword*في المستند باستخدام خيارات البحث (التعبير العادي ، حالة المطابقة ، إلخ.) .

```csharp
public IEnumerable<SearchResult> Search(string keyword, SearchOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| keyword | String | الكلمة الرئيسية للبحث. |
| options | SearchOptions | خيارات البحث. |

### قيمة الإرجاع

مجموعة من[`SearchResult`](../../../groupdocs.parser.data/searchresult) كائنات ؛ `لا شيء` إذا لم يتم دعم البحث.

### ملاحظات

**يتعلم أكثر:**

* [نص البحث](https://docs.groupdocs.com/display/parsernet/Search+text)
* [ابحث عن نص في مستندات Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [ابحث عن نص في جداول بيانات Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [نص البحث في عروض Microsoft Office PowerPoint التقديمية](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [ابحث عن نص في مستندات PDF](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [نص البحث في رسائل البريد الإلكتروني](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [البحث عن نص في الكتب الإلكترونية EPUB](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [نص البحث في مستندات HTML](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [ابحث عن نص في أقسام Microsoft OneNote](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### أمثلة

يوضح المثال التالي كيفية البحث باستخدام تعبير عادي في مستند:

يوضح المثال التالي كيفية البحث عن نص في الصفحات:

```csharp
// إنشاء مثيل لفئة المحلل اللغوي
using(Parser parser = new Parser(filePath))
{
    // بحث باستخدام تعبير عادي مع مطابقة حالة الأحرف
    IEnumerable<SearchResult> sr = parser.Search("page number: [0-9]+", new SearchOptions(true, false, true));
    // تحقق مما إذا كان البحث مدعومًا
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // كرر عبر نتائج البحث
    foreach(SearchResult s in sr)
    {
        // طباعة فهرس والنص الذي تم العثور عليه:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

```csharp
// إنشاء مثيل لفئة المحلل اللغوي
using(Parser parser = new Parser(filePath))
{
    // ابحث عن كلمة رئيسية بأرقام الصفحات
    IEnumerable<SearchResult> sr = parser.Search("line", new SearchOptions(false, false, false, true));
    // تحقق مما إذا كان البحث مدعومًا
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // كرر عبر نتائج البحث
    foreach(SearchResult s in sr)
    {
        // طباعة فهرس ورقم الصفحة والنص الذي تم العثور عليه:
        Console.WriteLine(string.Format("At {0} (page {1}): {2}", s.Position, s.PageIndex, s.Text));
    }
}
```

### أنظر أيضا

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [SearchOptions](../../../groupdocs.parser.options/searchoptions)
* class [Parser](../../parser)
* مساحة الاسم [GroupDocs.Parser](../../parser)
* المجسم [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

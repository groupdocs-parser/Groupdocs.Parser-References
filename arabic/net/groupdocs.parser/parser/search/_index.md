---
title: "Search"
second_title: "GroupDocs.Parser لـ .NET API مرجع"
description: "يبحث عن كلمة مفتاحية في المستند."
type: docs
weight: 250
url: /ar/net/groupdocs.parser/parser/search/
---

## Search(string) {#search}

يبحث عن *keyword* في المستند.

```csharp
public IEnumerable<SearchResult> Search(string keyword)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| كلمة مفتاحية | سلسلة | الكلمة المفتاحية للبحث. |

### قيمة الإرجاع

مجموعة من كائنات [`SearchResult`](../../../groupdocs.parser.data/searchresult)؛ `null` إذا لم يكن البحث مدعومًا.

### ملاحظات

**Learn more:**

* [Search text](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Search text in Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Search text in Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Search text in Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Search text in PDF documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Search text in Emails](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Search text in EPUB eBooks](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Search text in HTML documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Search text in Microsoft OneNote sections](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### أمثلة

المثال التالي يوضح كيفية العثور على كلمة مفتاحية في مستند:

```csharp
// إنشاء مثال من فئة Parser
using(Parser parser = new Parser(filePath))
{
    // ابحث عن كلمة مفتاحية:
    IEnumerable<SearchResult> sr = parser.Search("page number");
    // تحقق مما إذا كان البحث مدعومًا
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // تكرار عبر نتائج البحث
    foreach(SearchResult s in sr)
    {
        // طباعة الفهرس والنص الموجود:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

### انظر أيضًا

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Search(string, SearchOptions) {#search_1}

يبحث عن *keyword* في المستند باستخدام خيارات البحث (التعبير النمطي، مطابقة الحالة، إلخ).

```csharp
public IEnumerable<SearchResult> Search(string keyword, SearchOptions options)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| كلمة مفتاحية | سلسلة | الكلمة المفتاحية للبحث. |
| options | SearchOptions | خيارات البحث. |

### قيمة الإرجاع

مجموعة من كائنات [`SearchResult`](../../../groupdocs.parser.data/searchresult)؛ `null` إذا لم يكن البحث مدعومًا.

### ملاحظات

**Learn more:**

* [Search text](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Search text in Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Search text in Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Search text in Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Search text in PDF documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Search text in Emails](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Search text in EPUB eBooks](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Search text in HTML documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Search text in Microsoft OneNote sections](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### أمثلة

المثال التالي يوضح كيفية البحث باستخدام تعبير عادي في مستند:

```csharp
// إنشاء مثال من فئة Parser
using(Parser parser = new Parser(filePath))
{
    // البحث باستخدام تعبير عادي مع مطابقة الحالة
    IEnumerable<SearchResult> sr = parser.Search("page number: [0-9]+", new SearchOptions(true, false, true));
    // تحقق مما إذا كان البحث مدعومًا
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // تكرار عبر نتائج البحث
    foreach(SearchResult s in sr)
    {
        // طباعة الفهرس والنص الموجود:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

المثال التالي يوضح كيفية البحث عن نص في الصفحات:

```csharp
// إنشاء مثال من فئة Parser
using(Parser parser = new Parser(filePath))
{
    // البحث عن كلمة مفتاحية مع أرقام الصفحات
    IEnumerable<SearchResult> sr = parser.Search("line", new SearchOptions(false, false, false, true));
    // تحقق مما إذا كان البحث مدعومًا
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // تكرار عبر نتائج البحث
    foreach(SearchResult s in sr)
    {
        // طباعة الفهرس، رقم الصفحة والنص الموجود:
        Console.WriteLine(string.Format("At {0} (page {1}): {2}", s.Position, s.PageIndex, s.Text));
    }
}
```

### انظر أيضًا

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [SearchOptions](../../../groupdocs.parser.options/searchoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

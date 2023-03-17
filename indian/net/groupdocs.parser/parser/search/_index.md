---
title: Search
second_title: GroupDocs.Parser .NET API संदर्भ के लिए
description: खजत हैkeyword दस्तवेज़ में.
type: docs
weight: 200
url: /hi/net/groupdocs.parser/parser/search/
---
## Search(string) {#search}

खोजता है*keyword* दस्तावेज़ में.

```csharp
public IEnumerable<SearchResult> Search(string keyword)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| keyword | String | खोज करने के लिए कीवर्ड। |

### प्रतिलाभ की मात्रा

का संग्रह[`SearchResult`](../../../groupdocs.parser.data/searchresult) वस्तुएं; `व्यर्थ` यदि खोज समर्थित नहीं है.

### टिप्पणियों

**और अधिक जानें:**

* [पाठ खोजें](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Microsoft Office Word दस्तावेज़ों में टेक्स्ट खोजें](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Microsoft Office Excel स्प्रेडशीट्स में टेक्स्ट खोजें](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Microsoft Office PowerPoint प्रस्तुतियों में पाठ खोजें](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [पीडीएफ दस्तावेजों में टेक्स्ट खोजें](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [ईमेल में पाठ खोजें](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [EPUB ईपुस्तकों में टेक्स्ट खोजें](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [HTML दस्तावेज़ों में टेक्स्ट खोजें](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Microsoft OneNote अनुभागों में पाठ खोजें](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### उदाहरण

निम्न उदाहरण दिखाता है कि दस्तावेज़ में कीवर्ड कैसे खोजें:

```csharp
// पार्सर वर्ग का एक उदाहरण बनाएँ
using(Parser parser = new Parser(filePath))
{
    // कीवर्ड खोजें:
    IEnumerable<SearchResult> sr = parser.Search("page number");
    // जांचें कि क्या खोज समर्थित है
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // खोज परिणामों पर पुनरावृति करें
    foreach(SearchResult s in sr)
    {
        // एक इंडेक्स प्रिंट करें और टेक्स्ट मिला:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

### यह सभी देखें

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

---

## Search(string, SearchOptions) {#search_1}

खोजता है*keyword*दस्तावेज़ में खोज विकल्प (रेगुलर एक्सप्रेशन, मैच केस, आदि) का उपयोग करके .

```csharp
public IEnumerable<SearchResult> Search(string keyword, SearchOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| keyword | String | खोज करने के लिए कीवर्ड। |
| options | SearchOptions | खोज विकल्प। |

### प्रतिलाभ की मात्रा

का संग्रह[`SearchResult`](../../../groupdocs.parser.data/searchresult) ऑब्जेक्ट्स; `व्यर्थ` यदि खोज समर्थित नहीं है.

### टिप्पणियों

**और अधिक जानें:**

* [पाठ खोजें](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Microsoft Office Word दस्तावेज़ों में टेक्स्ट खोजें](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Microsoft Office Excel स्प्रेडशीट्स में टेक्स्ट खोजें](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Microsoft Office PowerPoint प्रस्तुतियों में पाठ खोजें](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [पीडीएफ दस्तावेजों में टेक्स्ट खोजें](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [ईमेल में पाठ खोजें](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [EPUB ईपुस्तकों में टेक्स्ट खोजें](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [HTML दस्तावेज़ों में टेक्स्ट खोजें](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Microsoft OneNote अनुभागों में पाठ खोजें](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### उदाहरण

निम्न उदाहरण दिखाता है कि किसी दस्तावेज़ में रेगुलर एक्सप्रेशन के साथ कैसे खोजा जाए:

निम्न उदाहरण दिखाता है कि पृष्ठों पर टेक्स्ट कैसे खोजें:

```csharp
// पार्सर वर्ग का एक उदाहरण बनाएँ
using(Parser parser = new Parser(filePath))
{
    // केस मैचिंग के साथ रेगुलर एक्सप्रेशन से खोजें
    IEnumerable<SearchResult> sr = parser.Search("page number: [0-9]+", new SearchOptions(true, false, true));
    // जांचें कि क्या खोज समर्थित है
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // खोज परिणामों पर पुनरावृति करें
    foreach(SearchResult s in sr)
    {
        // एक इंडेक्स प्रिंट करें और टेक्स्ट मिला:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

```csharp
// पार्सर वर्ग का एक उदाहरण बनाएँ
using(Parser parser = new Parser(filePath))
{
    // पेज नंबर के साथ एक कीवर्ड खोजें
    IEnumerable<SearchResult> sr = parser.Search("line", new SearchOptions(false, false, false, true));
    // जांचें कि क्या खोज समर्थित है
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // खोज परिणामों पर पुनरावृति करें
    foreach(SearchResult s in sr)
    {
        // एक इंडेक्स, पेज नंबर और पाया गया टेक्स्ट प्रिंट करें:
        Console.WriteLine(string.Format("At {0} (page {1}): {2}", s.Position, s.PageIndex, s.Text));
    }
}
```

### यह सभी देखें

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [SearchOptions](../../../groupdocs.parser.options/searchoptions)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

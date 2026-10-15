---
title: "Search"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "दस्तावेज़ में एक कुंजीशब्द खोजता है।"
type: docs
weight: 250
url: /hi/net/groupdocs.parser/parser/search/
---

## Search(string) {#search}

दस्तावेज़ में एक *keyword* खोजता है।

```csharp
public IEnumerable<SearchResult> Search(string keyword)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कीवर्ड | स्ट्रिंग | खोजने के लिए कीवर्ड। |

### रिटर्न वैल्यू

एक संग्रह जिसमें [`SearchResult`](../../../groupdocs.parser.data/searchresult) ऑब्जेक्ट्स हैं; यदि खोज समर्थित नहीं है तो `null`।

### टिप्पणियाँ

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

### Examples

निम्नलिखित उदाहरण दिखाता है कि दस्तावेज़ में कीवर्ड कैसे पाया जाए:

```csharp
// Parser class का एक instance बनाएं
using(Parser parser = new Parser(filePath))
{
    // कीवर्ड खोजें:
    IEnumerable<SearchResult> sr = parser.Search("page number");
    // जाँचें कि खोज समर्थित है या नहीं
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // खोज परिणामों पर पुनरावृति करें
    foreach(SearchResult s in sr)
    {
        // एक अनुक्रमांक और पाए गए पाठ को प्रिंट करें:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

### संबंधित देखें

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Search(string, SearchOptions) {#search_1}

दस्तावेज़ में एक *keyword* खोजता है, खोज विकल्पों का उपयोग करके (रेगुलर एक्सप्रेशन, केस मिलान, आदि)।

```csharp
public IEnumerable<SearchResult> Search(string keyword, SearchOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कीवर्ड | स्ट्रिंग | खोजने के लिए कीवर्ड। |
| options | SearchOptions | खोज विकल्प। |

### रिटर्न वैल्यू

एक संग्रह जिसमें [`SearchResult`](../../../groupdocs.parser.data/searchresult) ऑब्जेक्ट्स हैं; यदि खोज समर्थित नहीं है तो `null`।

### टिप्पणियाँ

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

### Examples

निम्नलिखित उदाहरण दिखाता है कि दस्तावेज़ में नियमित अभिव्यक्ति के साथ कैसे खोजें:

```csharp
// Parser class का एक instance बनाएं
using(Parser parser = new Parser(filePath))
{
    // केस मिलान के साथ नियमित अभिव्यक्ति से खोजें
    IEnumerable<SearchResult> sr = parser.Search("page number: [0-9]+", new SearchOptions(true, false, true));
    // जाँचें कि खोज समर्थित है या नहीं
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // खोज परिणामों पर पुनरावृति करें
    foreach(SearchResult s in sr)
    {
        // एक अनुक्रमांक और पाए गए पाठ को प्रिंट करें:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

निम्नलिखित उदाहरण दिखाता है कि पृष्ठों पर पाठ कैसे खोजें:

```csharp
// Parser class का एक instance बनाएं
using(Parser parser = new Parser(filePath))
{
    // पृष्ठ संख्याओं के साथ कीवर्ड खोजें
    IEnumerable<SearchResult> sr = parser.Search("line", new SearchOptions(false, false, false, true));
    // जाँचें कि खोज समर्थित है या नहीं
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // खोज परिणामों पर पुनरावृति करें
    foreach(SearchResult s in sr)
    {
        // एक अनुक्रमांक, पृष्ठ संख्या और पाए गए पाठ को प्रिंट करें:
        Console.WriteLine(string.Format("At {0} (page {1}): {2}", s.Position, s.PageIndex, s.Text));
    }
}
```

### संबंधित देखें

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [SearchOptions](../../../groupdocs.parser.options/searchoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->

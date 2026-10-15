---
title: "GetToc"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "दस्तावेज़ से सामग्री तालिका निकालता है।"
type: docs
weight: 200
url: /hi/net/groupdocs.parser/parser/gettoc/
---

## Parser.GetToc method

दस्तावेज़ से सामग्री तालिका निकालता है।

```csharp
public IEnumerable<TocItem> GetToc()
```

### रिटर्न वैल्यू

सामग्री-सूची आइटम्स का संग्रह; `null` यदि सामग्री-सूची निष्कर्षण समर्थित नहीं है।

### टिप्पणियाँ

**Learn more:**

* [Extract table of contents](https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents)
* [Extract text by table of contents item](https://docs.groupdocs.com/display/parsernet/Extract+text+by+table+of+contents+item)
* [Extract table of contents from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents+from+Microsoft+Office+Word+documents)
* [Extract table of contents from EPUB eBooks](https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents+from+EPUB+eBooks)

### Examples

निम्नलिखित उदाहरण दिखाता है कि CHM फ़ाइल से सामग्री‑सूची कैसे निकाली जाए:

```csharp
// Parser class का एक instance बनाएं
using (Parser parser = new Parser(filePath))
{
    // जाँचें कि क्या पाठ निष्कर्षण समर्थित है
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }

    // जाँचें कि toc निष्कर्षण समर्थित है या नहीं
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
 
    // तालिका सामग्री प्राप्त करें
    IEnumerable<TocItem> toc = parser.GetToc();
    
    // आइटम्स पर पुनरावृति करें
    foreach (TocItem i in toc)
    {
        // Toc पाठ को प्रिंट करें
        Console.WriteLine(i.Text);
        // जाँचें कि पृष्ठ अनुक्रमांक में कोई मान है या नहीं
        if (i.PageIndex == null)
        {
            continue;
        }
        // एक पृष्ठ का पाठ निकालें
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### संबंधित देखें

* class [TocItem](../../../groupdocs.parser.data/tocitem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->

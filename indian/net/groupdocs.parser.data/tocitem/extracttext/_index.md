---
title: "ExtractText"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "TocItemgroupdocs.parser.data/tocitem object को संदर्भित करने वाले दस्तावेज़ से एक टेक्स्ट निकालता है।"
type: docs
weight: 50
url: /hi/net/groupdocs.parser.data/tocitem/extracttext/
---

## TocItem.ExtractText method

[`TocItem`](../../tocitem) object को संदर्भित करने वाले दस्तावेज़ से एक टेक्स्ट निकालता है।

```csharp
public virtual TextReader ExtractText()
```

### रिटर्न वैल्यू

निकाले गए टेक्स्ट के साथ TextReader class का एक instance।

### Examples

निम्न उदाहरण दर्शाता है कि तालिका सामग्री के एक आइटम द्वारा टेक्स्ट कैसे निकाला जाए:

```csharp
// Parser class का एक instance बनाएं
using (Parser parser = new Parser(Constants.SampleDocxWithToc))
{
    // तालिका सामग्री प्राप्त करें
    IEnumerable<TocItem> tocItems = parser.GetToc();
    // जाँचें कि toc निष्कर्षण समर्थित है या नहीं
    if (tocItems == null)
    {
        Console.WriteLine("Table of contents extraction isn't supported");
    }
    // आइटम्स पर पुनरावृति करें
    foreach (TocItem tocItem in tocItems)
    {
        // अध्याय का पाठ प्रिंट करें
        using (TextReader reader = tocItem.ExtractText())
        {
            Console.WriteLine("----");
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### संबंधित देखें

* class [TocItem](../../tocitem)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->

---
title: "GetHighlight"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "दस्तावेज़ से हाइलाइट निकालता है।"
type: docs
weight: 110
url: /hi/net/groupdocs.parser/parser/gethighlight/
---

## Parser.GetHighlight method

दस्तावेज़ से हाइलाइट निकालता है।

```csharp
public HighlightItem GetHighlight(int position, bool isDirect, HighlightOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्थिति | Int32 | हाइलाइट की प्रारंभिक स्थिति। |
| isDirect | Boolean | वह मान जो दर्शाता है कि हाइलाइट निष्कर्षण प्रत्यक्ष है या नहीं। `true` यदि हाइलाइट *स्थिति* के दाएँ से निकाला गया हो; अन्यथा, `false`। |
| options | HighlightOptions | हाइलाइट निष्कर्षण विकल्प। |

### रिटर्न वैल्यू

एक उदाहरण [`HighlightItem`](../../../groupdocs.parser.data/highlightitem) क्लास का जो निकाले गए हाइलाइट को दर्शाता है; `null` यदि हाइलाइट निष्कर्षण समर्थित नहीं है।

### टिप्पणियाँ

**Learn more:**

* [Extract highlights](https://docs.groupdocs.com/display/parsernet/Extract+highlights)

### Examples

निम्न उदाहरण दिखाता है कि 3 शब्दों वाला हाइलाइट कैसे निकाला जाए:

```csharp
// Parser class का एक instance बनाएं
using (Parser parser = new Parser(filePath))
{
    // हाइलाइट निकालें:
    HighlightItem hl = parser.GetHighlight(2, true, new HighlightOptions(3));
    
    // जाँचें कि हाइलाइट निष्कर्षण समर्थित है या नहीं
    if (hl == null)
    {
        Console.WriteLine("Highlight extraction isn't supported");
        return;
    }
    
    // निकाले गए हाइलाइट को प्रिंट करें
    Console.WriteLine(string.Format("At {0}: {1}", hl.Position, hl.Text));
}
```

### संबंधित देखें

* class [HighlightItem](../../../groupdocs.parser.data/highlightitem)
* class [HighlightOptions](../../../groupdocs.parser.options/highlightoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->

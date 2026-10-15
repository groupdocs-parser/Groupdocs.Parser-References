---
title: "GetMetadata"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "दस्तावेज़ से मेटाडेटा निकालता है।"
type: docs
weight: 140
url: /hi/net/groupdocs.parser/parser/getmetadata/
---

## Parser.GetMetadata method

दस्तावेज़ से मेटाडेटा निकालता है।

```csharp
public IEnumerable<MetadataItem> GetMetadata()
```

### रिटर्न वैल्यू

मेटाडेटा आइटम्स का संग्रह; यदि मेटाडेटा निष्कर्षण समर्थित नहीं है तो `null`।

### टिप्पणियाँ

**Learn more:**

* [Extract metadata from documents](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+documents)
* [Extract metadata from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+Word+documents)
* [Extract metadata from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+Excel+spreadsheets)
* [Extract metadata from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+PowerPoint+presentations)
* [Extract metadata from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+PDF+documents)
* [Extract metadata from Emails](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Emails)

### Examples

निम्न उदाहरण दिखाता है कि कैसे दस्तावेज़ से मेटाडेटा निकाला जाए:

```csharp
// Parser class का एक instance बनाएं
using(Parser parser = new Parser(filePath))
{
    // दस्तावेज़ से मेटाडेटा निकालें
    IEnumerable<MetadataItem> metadata = parser.GetMetadata();
    // जाँचें कि क्या मेटाडेटा निष्कर्षण समर्थित है
    if(metadata == null)
    {
        Console.WriteLine("Metatada extraction isn't supported");
    }
 
    // मेटाडेटा आइटम्स पर पुनरावृति करें
    foreach(MetadataItem item in metadata)
    {
        // आइटम का नाम और मान प्रिंट करें
        Console.WriteLine(string.Format("{0}: {1}", item.Name, item.Value));
    }
}
```

### संबंधित देखें

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->

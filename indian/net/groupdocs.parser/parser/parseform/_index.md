---
title: "ParseForm"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "दस्तावेज़ फ़ॉर्म को पार्स करता है।"
type: docs
weight: 240
url: /hi/net/groupdocs.parser/parser/parseform/
---

## Parser.ParseForm method

दस्तावेज़ फ़ॉर्म को पार्स करता है।

```csharp
public DocumentData ParseForm()
```

### रिटर्न वैल्यू

[`DocumentData`](../../../groupdocs.parser.data/documentdata) वर्ग का एक उदाहरण जो निकाले गए डेटा को रखता है; `null` यदि टेम्प्लेट द्वारा पार्सिंग समर्थित नहीं है।

### टिप्पणियाँ

**Learn more:**

* [Extract data from PDF forms](https://docs.groupdocs.com/display/parsernet/Extract+data+from+PDF+forms)
* [Working with extracted data](https://docs.groupdocs.com/display/parsernet/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+PDF+documents)

### Examples

निम्नलिखित उदाहरण दिखाता है कि दस्तावेज़ के एक रूप को कैसे पार्स किया जाए:

```csharp
// Parser class का एक instance बनाएं
using (Parser parser = new Parser(filePath))
{
    // PDF दस्तावेज़ से डेटा निकालें
    DocumentData data = parser.ParseForm();
    // निकाले गए डेटा पर इटररेट करें
    for (int i = 0; i<data.Count; i++)
    {
        Console.Write(data[i].Name + ": ");
        PageTextArea area = data[i].PageArea as PageTextArea;
        Console.WriteLine(area == null ? "Not a template field" : area.Text);
    }
}
```

### संबंधित देखें

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->

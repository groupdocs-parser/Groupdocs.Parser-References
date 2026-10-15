---
title: "PageArea"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "फ़ील्ड का मान प्राप्त करता है।"
type: docs
weight: 30
url: /hi/net/groupdocs.parser.data/fielddata/pagearea/
---

## FieldData.PageArea property

फ़ील्ड का मान प्राप्त करता है।

```csharp
public PageArea PageArea { get; }
```

### Property Value

एक [`PageArea`](../../pagearea) क्लास का उदाहरण जो फ़ील्ड के मान को दर्शाता है।

### Examples

फ़ील्ड के `PageArea` प्रॉपर्टी के आधार पर यह [`PageArea`](../../pagearea) क्लास के किसी भी उत्तराधिकारी को सम्मिलित कर सकता है। उदाहरण के लिए, [`ParseForm`](../../../groupdocs.parser/parser/parseform) मेथड केवल टेक्स्ट फ़ील्ड निकालता है।

```csharp
// फ़ील्ड डेटा प्राप्त करें
FieldData field = data[i];
// जाँचें कि फ़ील्ड डेटा में कोई टेक्स्ट है या नहीं
if(field.PageArea is PageTextArea)
{
    // फ़ील्ड टेक्स्ट मान प्रिंट करें
    Console.WriteLine(field.Text);
}
```

### संबंधित देखें

* class [PageArea](../../pagearea)
* class [FieldData](../../fielddata)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->

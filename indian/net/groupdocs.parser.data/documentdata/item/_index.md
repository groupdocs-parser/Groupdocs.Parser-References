---
title: "आइटम"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "इंडेक्स द्वारा फ़ील्ड डेटा प्राप्त करता है।"
type: docs
weight: 20
url: /hi/net/groupdocs.parser.data/documentdata/item/
---

## DocumentData indexer

इंडेक्स द्वारा फ़ील्ड डेटा प्राप्त करता है।

```csharp
public FieldData this[int index] { get; }
```

| पैरामीटर | विवरण |
| --- | --- |
| index | फ़ील्ड का शून्य-आधारित सूचकांक। |

### रिटर्न वैल्यू

[`FieldData`](../../fielddata) क्लास का एक उदाहरण।

### Examples

सभी फ़ील्ड्स के माध्यम से इटरेशन:

```csharp
for (int i = 0; i < data.Count; i++)
{
    Console.Write(data[i].Name + ": ");
    PageTextArea area = data[i].PageArea as PageTextArea;
    Console.WriteLine(area == null ? "Not a template field" : area.Text);
}
```

[`FieldData`](../../fielddata) class represents field data. Depending on the field [`PageArea`](../../fielddata/pagearea) property can contain any of the inheritors of [`PageArea`](../../pagearea) class. For example, [`ParseForm`](../../../groupdocs.parser/parser/parseform) method extracts only text fields:

```csharp
// पार्सर बनाएं
using (Parser parser = new Parser(filePath))
{
    // PDF फ़ॉर्म से डेटा निकालें
    DocumentData data = parser.ParseForm();
    // निकाले गए फ़ील्ड्स पर इटररेट करें
    for (int i = 0; i < data.Count; i++)
    {
        // निकाला गया फ़ील्ड प्राप्त करें
        FieldData field = data[i];
        // फ़ील्ड का नाम प्रिंट करें
        Console.Write(field.Name + ": ");
        // जाँचें कि फ़ील्ड मान टेक्स्ट है या नहीं और उसे प्रिंट करें
        PageTextArea area = field.PageArea as PageTextArea;
        Console.WriteLine(area == null ? "Not a template field" : area.Text);
    }
}
```

### संबंधित देखें

* class [FieldData](../../fielddata)
* class [DocumentData](../../documentdata)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->

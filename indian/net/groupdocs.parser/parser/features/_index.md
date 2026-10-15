---
title: "Features"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "समर्थित सुविधाएँ प्राप्त करता है।"
type: docs
weight: 20
url: /hi/net/groupdocs.parser/parser/features/
---

## Parser.Features property

समर्थित सुविधाएँ प्राप्त करता है।

```csharp
public Features Features { get; }
```

### Property Value

एक उदाहरण [`Features`](../../../groupdocs.parser.options/features) क्लास का जो समर्थित सुविधाओं को दर्शाता है।

### टिप्पणियाँ

**Learn more:**

* [Get supported features](https://docs.groupdocs.com/display/parsernet/Get+supported+features)

### Examples

यदि सुविधा समर्थित नहीं है, तो मेथड मान के बजाय `null` लौटाता है। कुछ ऑपरेशनों में काफी समय लग सकता है। इसलिए केवल सुविधा समर्थन की जाँच करने के लिए मेथड को कॉल करना अनुकूल नहीं है। इस उद्देश्य के लिए Features प्रॉपर्टी का उपयोग किया जाता है:

```csharp
using(Parser parser = new Parser("doc.zip"))
{
    if(!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported");
        return;
    }
 
    using(TextReader reader = parser.GetText())
    {
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

### संबंधित देखें

* class [Features](../../../groupdocs.parser.options/features)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->

---
title: "GetDocumentInfo"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "दस्तावेज़ के बारे में सामान्य जानकारी लौटाता है।"
type: docs
weight: 90
url: /hi/net/groupdocs.parser/parser/getdocumentinfo/
---

## Parser.GetDocumentInfo method

दस्तावेज़ के बारे में सामान्य जानकारी लौटाता है।

```csharp
public IDocumentInfo GetDocumentInfo()
```

### रिटर्न वैल्यू

एक उदाहरण क्लास का जो [`IDocumentInfo`](../../../groupdocs.parser.options/idocumentinfo) इंटरफ़ेस को लागू करता है।

### टिप्पणियाँ

**Learn more:**

* [Get document info](https://docs.groupdocs.com/display/parsernet/Get+document+info)
* [Detect encoding](https://docs.groupdocs.com/display/parsernet/Detect+encoding)

### Examples

निम्नलिखित उदाहरण दिखाता है कि दस्तावेज़ जानकारी कैसे प्राप्त की जाए:

```csharp
// Parser class का एक instance बनाएं
using(Parser parser = new Parser(filePath))
{
    // दस्तावेज़ की जानकारी प्राप्त करें
    IDocumentInfo info = parser.GetDocumentInfo();

    Console.WriteLine(string.Format("FileType: {0}", info.FileType));
    Console.WriteLine(string.Format("PageCount: {0}", info.PageCount));
    Console.WriteLine(string.Format("Size: {0}", info.Size));
}
```

### संबंधित देखें

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->

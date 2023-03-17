---
title: GetDocumentInfo
second_title: GroupDocs.Parser .NET API संदर्भ के लिए
description: दस्तवेज़ के बरे में समन्य जनकर लटत है
type: docs
weight: 70
url: /hi/net/groupdocs.parser/parser/getdocumentinfo/
---
## Parser.GetDocumentInfo method

दस्तावेज़ के बारे में सामान्य जानकारी लौटाता है।

```csharp
public IDocumentInfo GetDocumentInfo()
```

### प्रतिलाभ की मात्रा

कक्षा का एक उदाहरण जो लागू होता है[`IDocumentInfo`](../../../groupdocs.parser.options/idocumentinfo) इंटरफेस।

### टिप्पणियों

**और अधिक जानें:**

* [दस्तावेज़ जानकारी प्राप्त करें](https://docs.groupdocs.com/display/parsernet/Get+document+info)
* [एन्कोडिंग का पता लगाएं](https://docs.groupdocs.com/display/parsernet/Detect+encoding)

### उदाहरण

निम्न उदाहरण दिखाता है कि दस्तावेज़ जानकारी कैसे प्राप्त करें:

```csharp
// पार्सर वर्ग का एक उदाहरण बनाएँ
using(Parser parser = new Parser(filePath))
{
    // दस्तावेज़ की जानकारी प्राप्त करें
    IDocumentInfo info = parser.GetDocumentInfo();

    Console.WriteLine(string.Format("FileType: {0}", info.FileType));
    Console.WriteLine(string.Format("PageCount: {0}", info.PageCount));
    Console.WriteLine(string.Format("Size: {0}", info.Size));
}
```

### यह सभी देखें

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
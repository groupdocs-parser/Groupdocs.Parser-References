---
title: "RawPageCount"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "दस्तावेज़ के कच्चे पृष्ठों की कुल संख्या प्राप्त करता है।"
type: docs
weight: 40
url: /hi/net/groupdocs.parser.options/idocumentinfo/rawpagecount/
---

## IDocumentInfo.RawPageCount property

दस्तावेज़ के कच्चे पृष्ठों की कुल संख्या प्राप्त करता है।

```csharp
public int RawPageCount { get; }
```

### Property Value

कुल कच्चे पृष्ठों की संख्या दर्शाने वाला पूर्णांक मान।

### टिप्पणियाँ

`RawPageCount` प्रॉपर्टी का उपयोग करें, कच्चा टेक्स्ट निकालने के लिए [`PageCount`](../pagecount) प्रॉपर्टी के बजाय। कुछ दस्तावेज़ सटीक और कच्चे टेक्स्ट निष्कर्षण मोड में अलग पृष्ठ संख्याएँ रखते हैं। [`PageCount`](../pagecount) प्रॉपर्टी अतिरिक्त गणनाएँ कर सकती है जो कच्चे मोड में टेक्स्ट निष्कर्षण गति को प्रभावित करती हैं।

### संबंधित देखें

* interface [IDocumentInfo](../../idocumentinfo)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->

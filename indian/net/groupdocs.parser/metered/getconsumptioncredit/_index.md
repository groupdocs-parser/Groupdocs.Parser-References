---
title: "GetConsumptionCredit"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "उपयोग किए गए क्रेडिट की संख्या प्राप्त करता है।"
type: docs
weight: 30
url: /hi/net/groupdocs.parser/metered/getconsumptioncredit/
---

## Metered.GetConsumptionCredit method

उपयोग किए गए क्रेडिट की संख्या प्राप्त करता है।

```csharp
public static decimal GetConsumptionCredit()
```

### रिटर्न वैल्यू

एक दशमलव मान जो उपभोग क्रेडिट को दर्शाता है।

### Examples

निम्न उदाहरण दिखाता है कि उपभोग किए गए क्रेडिट की गिनती कैसे प्राप्त की जाए।

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);

decimal creditsConsumed = Metered.GetConsumptionCredit();
```

### संबंधित देखें

* class [Metered](../../metered)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->

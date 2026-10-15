---
title: "GetConsumptionQuantity"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "प्रोसेस किए गए MB की मात्रा प्राप्त करता है।"
type: docs
weight: 40
url: /hi/net/groupdocs.parser/metered/getconsumptionquantity/
---

## Metered.GetConsumptionQuantity method

प्रोसेस किए गए MB की मात्रा प्राप्त करता है।

```csharp
public static decimal GetConsumptionQuantity()
```

### रिटर्न वैल्यू

एक दशमलव मान जो उपभोग मात्रा को दर्शाता है।

### Examples

निम्न उदाहरण दिखाता है कि प्रोसेस किए गए एमबी की मात्रा कैसे प्राप्त की जाए।

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);

decimal mbProcessed = Metered.GetConsumptionQuantity();
```

### संबंधित देखें

* class [Metered](../../metered)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->

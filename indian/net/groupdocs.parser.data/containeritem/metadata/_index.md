---
title: "Metadata"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "मेटाडाटा आइटमों का संग्रह प्राप्त करता है।"
type: docs
weight: 30
url: /hi/net/groupdocs.parser.data/containeritem/metadata/
---

## ContainerItem.Metadata property

मेटाडाटा आइटमों का संग्रह प्राप्त करता है।

```csharp
public IEnumerable<MetadataItem> Metadata { get; }
```

### Property Value

एक संग्रह जिसमें [`MetadataItem`](../../metadataitem) ऑब्जेक्ट्स हैं; यदि मेटाडेटा सेट नहीं है तो खाली।

### टिप्पणियाँ

ये मेटाडेटा स्वयं कंटेनर तत्व से संबंधित हैं, न कि किसी दस्तावेज़ से। कंटेनर प्रकार के आधार पर मेटाडेटा में निम्नलिखित आइटम हो सकते हैं:

**Email Attachments**

**Name**

**Description**

**content-type**

अटैचमेंट सामग्री का MIME प्रकार।

**ZIP Archives**

**Name**

**Description**

**date**

ज़िप एंट्री द्वारा संकेतित फ़ाइल का अंतिम संशोधित समय और तिथि।

**disposition**

यह पता लगाने के लिए कि इमेज अटैचमेंट इनलाइन है या नहीं, 'disposition' मेटाडेटा का उपयोग किया जाता है। यदि यह मौजूद है, तो यह 'inline' या 'attachment' मान ले सकता है।

**Outlook Storage**

**Name**

**Description**

**date**

Outlook स्टोरेज आइटम का अंतिम संशोधित समय और तिथि।

**email-sender**

"sender" फ़ील्ड का मान।

**email-to**

"to" फ़ील्ड का मान।

**subject**

"subject" फ़ील्ड का मान।

### संबंधित देखें

* class [MetadataItem](../../metadataitem)
* class [ContainerItem](../../containeritem)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->

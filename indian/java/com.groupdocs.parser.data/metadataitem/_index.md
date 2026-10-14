---
title: "MetadataItem"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "मेटाडेटा आइटम का प्रतिनिधित्व करता है जिसका उपयोग कंटेनर आइटम और मेटाडेटा निष्कर्षण कार्यक्षमता में किया जाता है।"
type: docs
weight: 15
url: /hi/java/com.groupdocs.parser.data/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

मेटाडेटा आइटम का प्रतिनिधित्व करता है जिसका उपयोग कंटेनर आइटम और मेटाडेटा निष्कर्षण कार्यक्षमता में किया जाता है।

[MetadataItem](../../com.groupdocs.parser.data/metadataitem) क्लास का एक इंस्टेंस [Parser.getMetadata()](../../com.groupdocs.parser/parser#getMetadata--) मेथड के रिटर्न वैल्यू के रूप में उपयोग किया जाता है।
और इसे [ContainerItem.getMetadata()](../../com.groupdocs.parser.data/containeritem#getMetadata--) कलेक्शन में एक आइटम के रूप में उपयोग किया जाता है। वहाँ उपयोग के उदाहरण देखें।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [MetadataItem(String name, String value)](#MetadataItem-java.lang.String-java.lang.String-) | [MetadataItem](../../com.groupdocs.parser.data/metadataitem) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getName()](#getName--) | मेटाडाटा आइटम का नाम प्राप्त करता है। |
|
|  | [getValue()](#getValue--) | मेटाडाटा आइटम का मान प्राप्त करता है। |
|
### MetadataItem(String name, String value) {#MetadataItem-java.lang.String-java.lang.String-}
```
public MetadataItem(String name, String value)
```


[MetadataItem](../../com.groupdocs.parser.data/metadataitem) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | नाम | java.lang.String | मेटाडाटा आइटम का नाम। |
|
|  | मान | java.lang.String | मेटाडाटा आइटम का मान। |
|

### getName() {#getName--}
```
public String getName()
```


मेटाडाटा आइटम का नाम प्राप्त करता है।


**Returns:**
java.lang.String - एक स्ट्रिंग वैल्यू जो मेटाडाटा आइटम के नाम का प्रतिनिधित्व करती है।

### getValue() {#getValue--}
```
public String getValue()
```


मेटाडाटा आइटम का मान प्राप्त करता है।


**Returns:**
java.lang.String - एक स्ट्रिंग वैल्यू जो मेटाडाटा आइटम के मान का प्रतिनिधित्व करती है।


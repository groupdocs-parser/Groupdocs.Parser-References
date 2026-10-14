---
title: "TemplateItem"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "टेम्पलेट आइटम्स के लिए बेस एब्स्ट्रैक्ट क्लास प्रदान करता है।"
type: docs
weight: 14
url: /hi/java/com.groupdocs.parser.templates/templateitem/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplateItem
```

टेम्पलेट आइटम्स के लिए बेस एब्स्ट्रैक्ट क्लास प्रदान करता है।

क्लास के उत्तराधिकारी [TemplateItem](../../com.groupdocs.parser.templates/templateitem) को [Template](../../com.groupdocs.parser.templates/template) संग्रह में उपयोग किया जाता है।

## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | दिए गए कारक द्वारा सभी निर्देशांक को स्केल करके वर्तमान आइटम की एक प्रति बनाता है। |
|
|  | [getName()](#getName--) | टेम्प्लेट आइटम का नाम प्राप्त करता है। |
|
|  | [getPageIndex()](#getPageIndex--) | टेम्प्लेट आइटम का पृष्ठ सूचकांक प्राप्त करता है। |
|
|  | [getPageWidth()](#getPageWidth--) | टेम्प्लेट आइटम बनाने के लिए उपयोग किए गए पृष्ठ की चौड़ाई प्राप्त करता है। |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | एक मान प्राप्त करता है जो दर्शाता है कि क्या  Name  को बड़े अक्षरों में बदला गया था। |
|
### scale(double factor) {#scale-double-}
```
public abstract TemplateItem scale(double factor)
```


दिए गए कारक द्वारा सभी निर्देशांक को स्केल करके वर्तमान आइटम की एक प्रति बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | फ़ैक्टर | double | स्केलिंग कारक। |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - A new [TemplateItem](../../com.groupdocs.parser.templates/templateitem) with scaled coordinates.

### getName() {#getName--}
```
public String getName()
```


टेम्प्लेट आइटम का नाम प्राप्त करता है।


**Returns:**
java.lang.String - एक अपरकेस स्ट्रिंग मान जो टेम्प्लेट आइटम के नाम को दर्शाता है।

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


टेम्प्लेट आइटम का पृष्ठ सूचकांक प्राप्त करता है।


**Returns:**
java.lang.Integer - एक पूर्णांक मान जो उस पृष्ठ के सूचकांक को दर्शाता है जहाँ टेम्प्लेट आइटम स्थित है;  null  यदि टेम्प्लेट आइटम किसी भी पृष्ठ पर स्थित है।

### getPageWidth() {#getPageWidth--}
```
public Double getPageWidth()
```


टेम्प्लेट आइटम बनाने के लिए उपयोग किए गए पृष्ठ की चौड़ाई प्राप्त करता है।


**Returns:**
java.lang.Double - पृष्ठ की चौड़ाई पिक्सेल में;  null  यदि पृष्ठ की चौड़ाई अज्ञात है।

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


एक मान प्राप्त करता है जो दर्शाता है कि क्या  Name  को बड़े अक्षरों में बदला गया था।


**Returns:**
boolean - एक बूलियन मान जो दर्शाता है कि क्या  Name  को बड़े अक्षरों में बदला गया था।


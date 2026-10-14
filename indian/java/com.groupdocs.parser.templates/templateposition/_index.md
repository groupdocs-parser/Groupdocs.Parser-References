---
title: "TemplatePosition"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "टेम्पलेट पोजीशन्स के लिए बेस एब्स्ट्रैक्ट क्लास प्रदान करता है।"
type: docs
weight: 18
url: /hi/java/com.groupdocs.parser.templates/templateposition/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplatePosition
```

टेम्पलेट पोजीशन्स के लिए बेस एब्स्ट्रैक्ट क्लास प्रदान करता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [TemplatePosition()](#TemplatePosition--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | दिए गए फ़ैक्टर द्वारा सभी निर्देशांक को स्केल करके वर्तमान स्थिति की एक कॉपी बनाता है। |
|
### TemplatePosition() {#TemplatePosition--}
```
public TemplatePosition()
```


### scale(double factor) {#scale-double-}
```
public abstract TemplatePosition scale(double factor)
```


दिए गए फ़ैक्टर द्वारा सभी निर्देशांक को स्केल करके वर्तमान स्थिति की एक कॉपी बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | फ़ैक्टर | double | स्केलिंग कारक। |
|

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - A new [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) with scaled coordinates.


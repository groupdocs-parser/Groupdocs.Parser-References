---
title: "PageArea"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "टेम्प्लेट द्वारा पार्सिंग कार्यक्षमता में दस्तावेज़ पृष्ठ पर ब्लॉकों को दर्शाने के लिए उपयोग किए जाने वाले पृष्ठ क्षेत्रों के लिए एक एब्स्ट्रैक्ट बेस क्लास का प्रतिनिधित्व करता है।"
type: docs
weight: 17
url: /hi/java/com.groupdocs.parser.data/pagearea/
---
**Inheritance:**
java.lang.Object
```
public abstract class PageArea
```

टेम्प्लेट द्वारा पार्सिंग कार्यक्षमता में दस्तावेज़ पृष्ठ पर ब्लॉकों को दर्शाने के लिए उपयोग किए जाने वाले पृष्ठ क्षेत्रों के लिए एक एब्स्ट्रैक्ट बेस क्लास का प्रतिनिधित्व करता है।

## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | आयताकार क्षेत्र प्राप्त करता है। |
|
|  | [getPage()](#getPage--) | दस्तावेज़ पृष्ठ जानकारी प्राप्त करता है जैसे पृष्ठ सूचकांक और पृष्ठ आकार। |
|
### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


आयताकार क्षेत्र प्राप्त करता है।


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area of the page that contains the page area.

### getPage() {#getPage--}
```
public Page getPage()
```


दस्तावेज़ पृष्ठ जानकारी प्राप्त करता है जैसे पृष्ठ सूचकांक और पृष्ठ आकार।


**Returns:**
[Page](../../com.groupdocs.parser.data/page) - An instance of [Page](../../com.groupdocs.parser.data/page) class that represents the page that contains the page area.


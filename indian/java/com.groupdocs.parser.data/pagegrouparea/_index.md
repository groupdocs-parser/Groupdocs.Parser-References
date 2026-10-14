---
title: "PageGroupArea"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "टेम्प्लेट द्वारा पार्सिंग कार्यक्षमता में दस्तावेज़ पृष्ठ के विभिन्न प्रकार के ब्लॉकों को समूहित करने के लिए उपयोग किए जाने वाले पृष्ठ क्षेत्रों के समूह का प्रतिनिधित्व करता है।"
type: docs
weight: 19
url: /hi/java/com.groupdocs.parser.data/pagegrouparea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageGroupArea extends PageArea
```

टेम्प्लेट द्वारा पार्सिंग कार्यक्षमता में दस्तावेज़ पृष्ठ के विभिन्न प्रकार के ब्लॉकों को समूहित करने के लिए उपयोग किए जाने वाले पृष्ठ क्षेत्रों के समूह का प्रतिनिधित्व करता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [PageGroupArea(Iterable<PageArea> areas, Page page)](#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-) | [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getAreas()](#getAreas--) | समूहित पृष्ठ क्षेत्रों का संग्रह प्राप्त करता है। |
|
### PageGroupArea(Iterable<PageArea> areas, Page page) {#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-}
```
public PageGroupArea(Iterable<PageArea> areas, Page page)
```


[PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | areas | java.lang.Iterable<com.groupdocs.parser.data.PageArea> | समूहित किए जाने वाले पृष्ठ क्षेत्रों का संग्रह। |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | वह पृष्ठ जिसमें यह क्षेत्र शामिल है। |
|

### getAreas() {#getAreas--}
```
public Iterable<PageArea> getAreas()
```


समूहित पृष्ठ क्षेत्रों का संग्रह प्राप्त करता है।


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageArea> - एक संग्रह [PageArea](../../com.groupdocs.parser.data/pagearea) ऑब्जेक्ट्स।


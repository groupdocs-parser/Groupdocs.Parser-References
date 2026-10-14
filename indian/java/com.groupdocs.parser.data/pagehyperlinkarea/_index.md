---
title: "PageHyperlinkArea"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "पृष्ठ पर हाइपरलिंक को दर्शाने के लिए उपयोग किए जाने वाले पृष्ठ क्षेत्र का प्रतिनिधित्व करता है।"
type: docs
weight: 20
url: /hi/java/com.groupdocs.parser.data/pagehyperlinkarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageHyperlinkArea extends PageArea
```

पृष्ठ पर हाइपरलिंक को दर्शाने के लिए उपयोग किए जाने वाले पृष्ठ क्षेत्र का प्रतिनिधित्व करता है।

निम्नलिखित विधियों के रिटर्न मान के रूप में [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) क्लास का एक उदाहरण उपयोग किया जाता है:

* [Parser.getHyperlinks()](../../com.groupdocs.parser/parser#getHyperlinks--)
* [Parser.getHyperlinks(PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-PageAreaOptions-)
* [Parser.getHyperlinks(int)](../../com.groupdocs.parser/parser#getHyperlinks-int-)
* [Parser.getHyperlinks(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-int--PageAreaOptions-)

वहाँ उपयोग उदाहरण देखें।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)](#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getText()](#getText--) | हाइपरलिंक पाठ प्राप्त करता है। |
|
|  | [getUrl()](#getUrl--) | हाइपरलिंक URL प्राप्त करता है। |
|
### PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle) {#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)
```


[PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) क्लास का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | पाठ | java.lang.String | हाइपरलिंक पाठ। |
|
|  | url | java.lang.String | हाइपरलिंक URL। |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | हाइपरलिंक वाले पृष्ठ। |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | हाइपरलिंक को सम्मिलित करने वाला आयताकार क्षेत्र। |
|

### getText() {#getText--}
```
public String getText()
```


हाइपरलिंक पाठ प्राप्त करता है।


**Returns:**
java.lang.String - हाइपरलिंक पाठ को दर्शाने वाला स्ट्रिंग मान।

### getUrl() {#getUrl--}
```
public String getUrl()
```


हाइपरलिंक URL प्राप्त करता है।


**Returns:**
java.lang.String - हाइपरलिंक URL को दर्शाने वाला स्ट्रिंग मान।


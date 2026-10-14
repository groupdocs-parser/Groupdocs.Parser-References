---
title: "PageTextArea"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "टेम्प्लेट या फॉर्म पार्सिंग कार्यक्षमता में टेक्स्ट मान को दर्शाने के लिए उपयोग किए जाने वाले पृष्ठ टेक्स्ट क्षेत्र का प्रतिनिधित्व करता है।"
type: docs
weight: 24
url: /hi/java/com.groupdocs.parser.data/pagetextarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTextArea extends PageArea
```

टेम्प्लेट या फॉर्म पार्सिंग कार्यक्षमता में टेक्स्ट मान को दर्शाने के लिए उपयोग किए जाने वाले पृष्ठ टेक्स्ट क्षेत्र का प्रतिनिधित्व करता है।

निम्नलिखित विधियों के लिए रिटर्न वैल्यू के रूप में [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) क्लास का एक उदाहरण उपयोग किया जाता है:

* [Parser.getTextAreas()](../../com.groupdocs.parser/parser#getTextAreas--)
* [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-)
* [Parser.getTextAreas(int)](../../com.groupdocs.parser/parser#getTextAreas-int-)
* [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-)

इसके अलावा, [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) क्लास का एक उदाहरण [PageArea](../../com.groupdocs.parser.data/pagearea) प्रॉपर्टी के मान के रूप में उपयोग किया जाता है।
\*

वहाँ उपयोग उदाहरण देखें।

टेक्स्ट एरिया एकल या संयुक्त हो सकता है। पहले मामले में इसमें एक टेक्स्ट होता है जो आयताकार क्षेत्र द्वारा सीमित होता है।
दूसरे मामले में इसमें अन्य टेक्स्ट एरिया होते हैं; टेक्स्ट और तालिका गुण बच्चों के टेक्स्ट एरिया द्वारा गणना किए जाते हैं।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [PageTextArea(String text, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) क्लास का नया उदाहरण प्रारंभ करता है। |
|
|  | [PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) क्लास का नया उदाहरण प्रारंभ करता है। |
|
|  | [PageTextArea(Iterable<PageTextArea> areas, Page page)](#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-) | [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) क्लास का नया उदाहरण प्रारंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getText()](#getText--) | टेक्स्ट प्राप्त करता है। |
|
|  | [getBaseLine()](#getBaseLine--) | बेस लाइन प्राप्त करता है। |
|
|  | [getTextStyle()](#getTextStyle--) | फ़ॉन्ट आकार, फ़ॉन्ट नाम आदि जैसी टेक्स्ट शैली प्राप्त करता है। |
|
|  | [getAreas()](#getAreas--) | चाइल्ड टेक्स्ट पेज एरिया का संग्रह प्राप्त करता है। |
|
### PageTextArea(String text, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Page page, Rectangle rectangle)
```


[PageTextArea](../../com.groupdocs.parser.data/pagetextarea) क्लास का नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | पाठ | java.lang.String | टेक्स्ट का मान। |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | टेक्स्ट एरिया को समाहित करने वाला पृष्ठ। |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | टेक्स्ट एरिया को समाहित करने वाला आयताकार क्षेत्र। |
|

### PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)
```


[PageTextArea](../../com.groupdocs.parser.data/pagetextarea) क्लास का नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | पाठ | java.lang.String | टेक्स्ट का मान। |
|
|  | baseLine | java.lang.Double | टेक्स्ट की बेस लाइन। |
|
|  | textStyle | [TextStyle](../../com.groupdocs.parser.data/textstyle) | टेक्स्ट की शैली। |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | टेक्स्ट एरिया को समाहित करने वाला पृष्ठ। |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | टेक्स्ट एरिया को समाहित करने वाला आयताकार क्षेत्र। |
|

### PageTextArea(Iterable<PageTextArea> areas, Page page) {#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-}
```
public PageTextArea(Iterable<PageTextArea> areas, Page page)
```


[PageTextArea](../../com.groupdocs.parser.data/pagetextarea) क्लास का नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | areas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea} | चाइल्ड टेक्स्ट पेज एरिया का संग्रह। |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | टेक्स्ट एरिया को समाहित करने वाला पृष्ठ। |
|

### getText() {#getText--}
```
public String getText()
```


टेक्स्ट प्राप्त करता है।


**Returns:**
java.lang.String - टेक्स्ट पेज एरिया के मान का प्रतिनिधित्व करने वाला एक स्ट्रिंग मान।

### getBaseLine() {#getBaseLine--}
```
public double getBaseLine()
```


बेस लाइन प्राप्त करता है।


**Returns:**
double - बेस लाइन का प्रतिनिधित्व करने वाला एक double मान।

### getTextStyle() {#getTextStyle--}
```
public TextStyle getTextStyle()
```


फ़ॉन्ट आकार, फ़ॉन्ट नाम आदि जैसी टेक्स्ट शैली प्राप्त करता है।


**Returns:**
[TextStyle](../../com.groupdocs.parser.data/textstyle) - An instance of [TextStyle](../../com.groupdocs.parser.data/textstyle) class that represents the text style.

### getAreas() {#getAreas--}
```
public List<PageTextArea> getAreas()
```


चाइल्ड टेक्स्ट पेज एरिया का संग्रह प्राप्त करता है।


**Returns:**
java.util.List<com.groupdocs.parser.data.PageTextArea> - चाइल्ड टेक्स्ट पेज एरिया का संग्रह; यदि टेक्स्ट पेज एरिया के कोई बच्चे नहीं हैं तो यह खाली रहेगा।


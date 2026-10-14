---
title: "Page"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "दस्तावेज़ पृष्ठ जानकारी का प्रतिनिधित्व करता है जैसे पृष्ठ सूचकांक और पृष्ठ आकार।"
type: docs
weight: 16
url: /hi/java/com.groupdocs.parser.data/page/
---
**Inheritance:**
java.lang.Object
```
public class Page
```

दस्तावेज़ पृष्ठ जानकारी का प्रतिनिधित्व करता है जैसे पृष्ठ सूचकांक और पृष्ठ आकार। यह टेम्पलेट फ़ंक्शनलिटी द्वारा पार्सिंग में [PageArea](../../com.groupdocs.parser.data/pagearea) क्लास के उत्तराधिकारियों को शामिल करने वाले पृष्ठ को दर्शाने के लिए उपयोग किया जाता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [Page(int index, Size size)](#Page-int-com.groupdocs.parser.data.Size-) | [Page](../../com.groupdocs.parser.data/page) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getIndex()](#getIndex--) | पेज इंडेक्स प्राप्त करता है। |
|
|  | [getSize()](#getSize--) | पृष्ठ आकार प्राप्त करता है। |
|
### Page(int index, Size size) {#Page-int-com.groupdocs.parser.data.Size-}
```
public Page(int index, Size size)
```


[Page](../../com.groupdocs.parser.data/page) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | इंडेक्स | int | पृष्ठ सूचकांक। |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | पृष्ठ आकार। |
|

### getIndex() {#getIndex--}
```
public int getIndex()
```


पेज इंडेक्स प्राप्त करता है।


**Returns:**
int - पृष्ठ का शून्य-आधारित सूचकांक।

### getSize() {#getSize--}
```
public Size getSize()
```


पृष्ठ आकार प्राप्त करता है।


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the page.


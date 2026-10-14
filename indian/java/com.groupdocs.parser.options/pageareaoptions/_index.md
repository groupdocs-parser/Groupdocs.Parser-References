---
title: "PageAreaOptions"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "पेज एरिया निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।"
type: docs
weight: 28
url: /hi/java/com.groupdocs.parser.options/pageareaoptions/
---
**Inheritance:**
java.lang.Object
```
public class PageAreaOptions
```

पेज एरिया निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।

[PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) क्लास का एक इंस्टेंस [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-) में पैरामीटर के रूप में उपयोग किया जाता है।
और [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-) मेथड्स। वहाँ उपयोग के उदाहरण देखें।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [PageAreaOptions(Rectangle rectangle)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-) | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) क्लास का नया इंस्टेंस अनदेखी सीमा के आकार के साथ प्रारंभ करता है। |
|
|  | [PageAreaOptions(Rectangle rectangle, double rectangleTolerance)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-) | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) क्लास का नया इंस्टेंस प्रारंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | पृष्ठ क्षेत्रों को सम्मिलित करने वाले आयताकार क्षेत्र को प्राप्त करता है। |
|
|  | [getRectangleTolerance()](#getRectangleTolerance--) | आयताकार क्षेत्र द्वारा कैप्चर किए जाने पर अनदेखी की जाने वाली सीमा का आकार प्राप्त करता है। |
|
### PageAreaOptions(Rectangle rectangle) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageAreaOptions(Rectangle rectangle)
```


[PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) क्लास का नया इंस्टेंस अनदेखी सीमा के आकार के साथ प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | पृष्ठ क्षेत्रों को सम्मिलित करने वाला आयताकार क्षेत्र। |
|

### PageAreaOptions(Rectangle rectangle, double rectangleTolerance) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-}
```
public PageAreaOptions(Rectangle rectangle, double rectangleTolerance)
```


[PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) क्लास का नया इंस्टेंस प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | पृष्ठ क्षेत्रों को सम्मिलित करने वाला आयताकार क्षेत्र। |
|
|  | rectangleTolerance | double | आयताकार क्षेत्र द्वारा कैप्चर किए जाने पर अनदेखी की जाने वाली सीमा का आकार। इसे टेक्स्ट आइटम की ऊँचाई के अंश द्वारा मापा जाता है। |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


पृष्ठ क्षेत्रों को सम्मिलित करने वाले आयताकार क्षेत्र को प्राप्त करता है।


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


आयताकार क्षेत्र द्वारा कैप्चर किए जाने पर अनदेखी की जाने वाली सीमा का आकार प्राप्त करता है। इसे टेक्स्ट आइटम की ऊँचाई के अंश द्वारा मापा जाता है।


**Returns:**
double - 0 (कोई सीमा नहीं) से 1 (पूरे तत्व को अनदेखा करें) तक का डबल मान।


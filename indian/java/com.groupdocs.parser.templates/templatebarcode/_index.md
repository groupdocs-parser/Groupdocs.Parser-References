---
title: "TemplateBarcode"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "टेम्पलेट बारकोड फ़ील्ड प्रदान करता है।"
type: docs
weight: 11
url: /hi/java/com.groupdocs.parser.templates/templatebarcode/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateBarcode extends TemplateItem
```

टेम्पलेट बारकोड फ़ील्ड प्रदान करता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [TemplateBarcode(Rectangle rectangle, String name)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-) | नया उदाहरण प्रारंभ करता है [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) वर्ग का। |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-) | नया उदाहरण प्रारंभ करता है [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) वर्ग का, UPPER CASE नाम के साथ। |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-) | नया उदाहरण प्रारंभ करता है [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) वर्ग का, UPPER CASE नाम के साथ। |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-) | नया उदाहरण प्रारंभ करता है [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) वर्ग का। |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | नया उदाहरण प्रारंभ करता है [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) वर्ग का। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | टेम्प्लेट बारकोड फ़ील्ड को सम्मिलित करने वाले आयताकार क्षेत्र को प्राप्त करता है। |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateBarcode(Rectangle rectangle, String name) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-}
```
public TemplateBarcode(Rectangle rectangle, String name)
```


नया उदाहरण प्रारंभ करता है [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) वर्ग का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | टेम्प्लेट बारकोड फ़ील्ड को सम्मिलित करने वाला आयताकार क्षेत्र। |
|
|  | नाम | java.lang.String | बारकोड फ़ील्ड का नाम। |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)
```


नया उदाहरण प्रारंभ करता है [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) वर्ग का, UPPER CASE नाम के साथ।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | टेम्प्लेट बारकोड फ़ील्ड को सम्मिलित करने वाला आयताकार क्षेत्र। |
|
|  | नाम | java.lang.String | बारकोड फ़ील्ड का नाम। |
|
|  | pageIndex | java.lang.Integer | एक पूर्णांक मान जो उस पृष्ठ का इंडेक्स दर्शाता है जहाँ टेम्प्लेट आइटम स्थित है; यदि टेम्प्लेट आइटम किसी भी पृष्ठ पर स्थित है तो null। |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)
```


नया उदाहरण प्रारंभ करता है [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) वर्ग का, UPPER CASE नाम के साथ।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | टेम्प्लेट बारकोड फ़ील्ड को सम्मिलित करने वाला आयताकार क्षेत्र। |
|
|  | नाम | java.lang.String | बारकोड फ़ील्ड का नाम। |
|
|  | pageIndex | java.lang.Integer | एक पूर्णांक मान जो उस पृष्ठ का इंडेक्स दर्शाता है जहाँ टेम्प्लेट आइटम स्थित है; यदि टेम्प्लेट आइटम किसी भी पृष्ठ पर स्थित है तो null। |
|
|  | pageWidth | java.lang.Double | पृष्ठ की चौड़ाई जिसका उपयोग टेम्पलेट आइटम बनाने के लिए किया गया था। |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)
```


नया उदाहरण प्रारंभ करता है [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) वर्ग का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | टेम्प्लेट बारकोड फ़ील्ड को सम्मिलित करने वाला आयताकार क्षेत्र। |
|
|  | नाम | java.lang.String | बारकोड फ़ील्ड का नाम। |
|
|  | pageIndex | java.lang.Integer | एक पूर्णांक मान जो उस पृष्ठ का इंडेक्स दर्शाता है जहाँ टेम्प्लेट आइटम स्थित है; यदि टेम्प्लेट आइटम किसी भी पृष्ठ पर स्थित है तो null। |
|
|  | useUpperCaseName | boolean | वह मान जो दर्शाता है कि क्या नाम को UPPER CASE में परिवर्तित किया गया है। |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


नया उदाहरण प्रारंभ करता है [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) वर्ग का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | टेम्प्लेट बारकोड फ़ील्ड को सम्मिलित करने वाला आयताकार क्षेत्र। |
|
|  | नाम | java.lang.String | बारकोड फ़ील्ड का नाम। |
|
|  | pageIndex | java.lang.Integer | एक पूर्णांक मान जो उस पृष्ठ का इंडेक्स दर्शाता है जहाँ टेम्प्लेट आइटम स्थित है; यदि टेम्प्लेट आइटम किसी भी पृष्ठ पर स्थित है तो null। |
|
|  | pageWidth | java.lang.Double | पृष्ठ की चौड़ाई जिसका उपयोग टेम्पलेट आइटम बनाने के लिए किया गया था। |
|
|  | useUpperCaseName | boolean | वह मान जो दर्शाता है कि क्या नाम को UPPER CASE में परिवर्तित किया गया है। |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


टेम्प्लेट बारकोड फ़ील्ड को सम्मिलित करने वाले आयताकार क्षेत्र को प्राप्त करता है।


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template barcode field.

### scale(double factor) {#scale-double-}
```
public TemplateItem scale(double factor)
```


दिए गए कारक द्वारा सभी निर्देशांक को स्केल करके वर्तमान आइटम की एक प्रति बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| फ़ैक्टर | double |  |

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem)

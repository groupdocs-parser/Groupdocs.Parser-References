---
title: "TemplateField"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "टेम्पलेट टेक्स्ट फ़ील्ड प्रदान करता है।"
type: docs
weight: 12
url: /hi/java/com.groupdocs.parser.templates/templatefield/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateField extends TemplateItem
```

टेम्पलेट टेक्स्ट फ़ील्ड प्रदान करता है।

पाठ फ़ील्ड पृष्ठ पर उसकी स्थिति द्वारा परिभाषित होते हैं। एक पाठ फ़ील्ड को परिभाषित करने के तीन तरीके हैं:

* Using the rectangular area: [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition)
* Using the regular expression: [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition)
* Using the linked field: [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition)

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [TemplateField(TemplatePosition position, String name)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-) | एक नया उदाहरण प्रारंभ करता है [TemplateField](../../com.groupdocs.parser.templates/templatefield) क्लास का। |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-) | एक नया उदाहरण प्रारंभ करता है [TemplateField](../../com.groupdocs.parser/templates/templatefield) क्लास का, जिसमें अपर केस नाम हो। |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-) | एक नया उदाहरण प्रारंभ करता है [TemplateField](../../com.groupdocs.parser/templates/templatefield) क्लास का, जिसमें अपर केस नाम हो। |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-) | एक नया उदाहरण प्रारंभ करता है [TemplateField](../../com.groupdocs.parser.templates/templatefield) क्लास का। |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | एक नया उदाहरण प्रारंभ करता है [TemplateField](../../com.groupdocs.parser.templates/templatefield) क्लास का। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getPosition()](#getPosition--) | डॉक्यूमेंट पेज पर टेम्प्लेट फ़ील्ड को खोजने के तरीके को वर्णित करने वाला मान प्राप्त करता है। |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateField(TemplatePosition position, String name) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-}
```
public TemplateField(TemplatePosition position, String name)
```


एक नया उदाहरण प्रारंभ करता है [TemplateField](../../com.groupdocs.parser.templates/templatefield) क्लास का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | फ़ील्ड की स्थिति। |
|
|  | नाम | java.lang.String | फ़ील्ड का नाम। |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex)
```


एक नया उदाहरण प्रारंभ करता है [TemplateField](../../com.groupdocs.parser/templates/templatefield) क्लास का, जिसमें अपर केस नाम हो।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | फ़ील्ड की स्थिति। |
|
|  | नाम | java.lang.String | फ़ील्ड का नाम। |
|
|  | pageIndex | java.lang.Integer | एक पूर्णांक मान जो उस पृष्ठ का इंडेक्स दर्शाता है जहाँ टेम्प्लेट आइटम स्थित है; यदि टेम्प्लेट आइटम किसी भी पृष्ठ पर स्थित है तो null। |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)
```


एक नया उदाहरण प्रारंभ करता है [TemplateField](../../com.groupdocs.parser/templates/templatefield) क्लास का, जिसमें अपर केस नाम हो।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | फ़ील्ड की स्थिति। |
|
|  | नाम | java.lang.String | फ़ील्ड का नाम। |
|
|  | pageIndex | java.lang.Integer | एक पूर्णांक मान जो उस पृष्ठ का इंडेक्स दर्शाता है जहाँ टेम्प्लेट आइटम स्थित है; यदि टेम्प्लेट आइटम किसी भी पृष्ठ पर स्थित है तो null। |
|
|  | pageWidth | java.lang.Double | पृष्ठ की चौड़ाई जिसका उपयोग टेम्पलेट आइटम बनाने के लिए किया गया था। |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)
```


एक नया उदाहरण प्रारंभ करता है [TemplateField](../../com.groupdocs.parser.templates/templatefield) क्लास का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | फ़ील्ड की स्थिति। |
|
|  | नाम | java.lang.String | फ़ील्ड का नाम। |
|
|  | pageIndex | java.lang.Integer | एक पूर्णांक मान जो उस पृष्ठ का इंडेक्स दर्शाता है जहाँ टेम्प्लेट आइटम स्थित है; यदि टेम्प्लेट आइटम किसी भी पृष्ठ पर स्थित है तो null। |
|
|  | useUpperCaseName | boolean | वह मान जो दर्शाता है कि क्या नाम को UPPER CASE में परिवर्तित किया गया है। |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


एक नया उदाहरण प्रारंभ करता है [TemplateField](../../com.groupdocs.parser.templates/templatefield) क्लास का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | फ़ील्ड की स्थिति। |
|
|  | नाम | java.lang.String | फ़ील्ड का नाम। |
|
|  | pageIndex | java.lang.Integer | एक पूर्णांक मान जो उस पृष्ठ का इंडेक्स दर्शाता है जहाँ टेम्प्लेट आइटम स्थित है; यदि टेम्प्लेट आइटम किसी भी पृष्ठ पर स्थित है तो null। |
|
|  | pageWidth | java.lang.Double | पृष्ठ की चौड़ाई जिसका उपयोग टेम्पलेट आइटम बनाने के लिए किया गया था। |
|
|  | useUpperCaseName | boolean | वह मान जो दर्शाता है कि क्या नाम को UPPER CASE में परिवर्तित किया गया है। |
|

### getPosition() {#getPosition--}
```
public TemplatePosition getPosition()
```


डॉक्यूमेंट पेज पर टेम्प्लेट फ़ील्ड को खोजने के तरीके को वर्णित करने वाला मान प्राप्त करता है।


**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - An instance of [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) descendant class.

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

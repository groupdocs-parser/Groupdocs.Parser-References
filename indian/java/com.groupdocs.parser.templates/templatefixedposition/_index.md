---
title: "TemplateFixedPosition"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "टेम्पलेट फ़ील्ड स्थिति प्रदान करता है जो आयताकार क्षेत्र द्वारा परिभाषित है।"
type: docs
weight: 13
url: /hi/java/com.groupdocs.parser.templates/templatefixedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateFixedPosition extends TemplatePosition
```

टेम्पलेट फ़ील्ड स्थिति प्रदान करता है जो आयताकार क्षेत्र द्वारा परिभाषित है।

फ़ील्ड की स्थिति निर्धारित करने का यह सबसे सरल तरीका है। यह पृष्ठ पर एक आयताकार क्षेत्र सेट करने की आवश्यकता रखता है जो सीमित करता है
फ़ील्ड मान को। आयताकार क्षेत्र में (भले ही आंशिक रूप से) सम्मिलित सभी पाठ को मान के रूप में निकाला जाएगा:

````
// Create a fixed template field with "Address" name which is bounded by a rectangle at the position (35, 160) and with the size (110, 20)
 TemplateField templateField = new TemplateField(
     new TemplateFixedPosition(new Rectangle(new Point(35, 160), new Size(110, 20))),
     "Address");
 
````


## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [TemplateFixedPosition(Rectangle rectangle)](#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-) | एक नया उदाहरण प्रारंभ करता है [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) क्लास का। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | टेम्प्लेट फ़ील्ड को सम्मिलित करने वाले आयताकार क्षेत्र को प्राप्त करता है। |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateFixedPosition(Rectangle rectangle) {#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-}
```
public TemplateFixedPosition(Rectangle rectangle)
```


एक नया उदाहरण प्रारंभ करता है [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) क्लास का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | टेम्प्लेट फ़ील्ड को सम्मिलित करने वाला आयताकार क्षेत्र। |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


टेम्प्लेट फ़ील्ड को सम्मिलित करने वाले आयताकार क्षेत्र को प्राप्त करता है।


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template field.

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


दिए गए फ़ैक्टर द्वारा सभी निर्देशांक को स्केल करके वर्तमान स्थिति की एक कॉपी बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| फ़ैक्टर | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)

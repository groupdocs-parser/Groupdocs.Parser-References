---
title: "TemplateTableLayout"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "टेम्प्लेट टेबल लेआउट प्रदान करता है जिसका उपयोग  क्लास द्वारा टेबल की स्थिति निर्धारित करने के लिए किया जाता है।"
type: docs
weight: 21
url: /hi/java/com.groupdocs.parser.templates/templatetablelayout/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableLayout
```

टेम्प्लेट टेबल लेआउट प्रदान करता है जिसका उपयोग [TemplateTable](../../com.groupdocs.parser.templates/templatetable) क्लास द्वारा टेबल की स्थिति निर्धारित करने के लिए किया जाता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)](#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--) | नया उदाहरण प्रारंभ करता है [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) क्लास का। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | टेबल को सम्मिलित करने वाले आयताकार क्षेत्र को प्राप्त करता है। |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | टेबल कॉलम विभाजकों को प्राप्त करता है। |
|
|  | [getHorizontalSeparators()](#getHorizontalSeparators--) | टेबल पंक्तियों के विभाजकों को प्राप्त करता है। |
|
|  | [moveTo(Point point)](#moveTo-com.groupdocs.parser.data.Point-) | एक ही आकार, विभाजक और बिंदु में स्थिति के साथ नया लेआउट बनाता है। |
|
|  | [scale(double factor)](#scale-double-) | दिए गए फ़ैक्टर द्वारा सभी निर्देशांक को स्केल करके इस लेआउट की एक कॉपी बनाता है। |
|
### TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators) {#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--}
```
public TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)
```


नया उदाहरण प्रारंभ करता है [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) क्लास का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | टेबल कॉलम विभाजक। |
|
|  | horizontalSeparators | java.lang.Iterable<java.lang.Double> | टेबल पंक्तियों के विभाजक। |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


टेबल को सम्मिलित करने वाले आयताकार क्षेत्र को प्राप्त करता है।


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


टेबल कॉलम विभाजकों को प्राप्त करता है।


**Returns:**
java.util.List<java.lang.Double> - एक संग्रह जिसमें डबल मान होते हैं जो टेबल कॉलम विभाजकों के x-निर्देशांक को दर्शाते हैं।

### getHorizontalSeparators() {#getHorizontalSeparators--}
```
public List<Double> getHorizontalSeparators()
```


टेबल पंक्तियों के विभाजकों को प्राप्त करता है।


**Returns:**
java.util.List<java.lang.Double> - एक संग्रह जिसमें डबल मान होते हैं जो टेबल पंक्तियों के विभाजकों के y-निर्देशांक को दर्शाते हैं।

### moveTo(Point point) {#moveTo-com.groupdocs.parser.data.Point-}
```
public TemplateTableLayout moveTo(Point point)
```


एक ही आकार, विभाजक और बिंदु में स्थिति के साथ नया लेआउट बनाता है।

यह कार्यक्षमता तालिका लेआउट को स्थानांतरित करने की अनुमति देती है।

उदाहरण के लिए, एक दस्तावेज़ में प्रत्येक पृष्ठ पर तालिकाएँ होती हैं (या पृष्ठ पर तालिका वाले दस्तावेज़ों का सेट)।
इन तालिकाओं की स्थिति और सामग्री में अंतर होता है, लेकिन इनके कॉलम और पंक्तियाँ समान होती हैं। इस मामले में उपयोगकर्ता
एक बार (0, 0) पर [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) ऑब्जेक्ट को परिभाषित कर सकते हैं और फिर इसे निश्चित तालिका के स्थान पर ले जा सकते हैं।

यदि तालिका की स्थिति पृष्ठ के अन्य ऑब्जेक्ट पर निर्भर करती है, तो उपयोगकर्ता [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) ऑब्जेक्ट को परिभाषित कर सकते हैं
टेम्पलेट दस्तावेज़ के आधार पर और फिर इसे एंकर ऑब्जेक्ट के अनुसार ले जा सकते हैं। उदाहरण के लिए, यदि यह एक सारांश तालिका है
और इसके बाद विवरण तालिका आती है (जिसमें पंक्तियों की संख्या अलग हो सकती है)। इस मामले में उपयोगकर्ता परिभाषित कर सकते हैं
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object on template document (with the known details table rectangle) and then move
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object according to the difference of details table rectangle of template and real document.


moveTo(Point)
विधि वर्तमान ऑब्जेक्ट की एक प्रति लौटाती है। उपयोगकर्ता कोई भी निर्देशांक पास कर सकते हैं
(भले ही नकारात्मक हों - तब लेआउट बाएँ/ऊपर की ओर स्थानांतरित हो जाएगा)।

````
// Create a table layout
 TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 0.0, 25.0, 150.0, 180.0, 230.0 }),
     java.util.Arrays.asList(new Double[] { 0.0, 15.0, 30.0, 45.0, 60.0, 75.0 }));
 // Print a rectangle
 Rectangle rect = layout.getRectangle();
 // Prints: pos: (0, 0) size: (230, 75)
 System.out.println(String.format("pos: (%d, %d) size: (%d, %d)",
         rect.getLeft(), rect.getTop(),
         rect.getSize().getWidth(), rect.getSize().getHeight()));
 // Move layout to the definite table location
 TemplateTableLayout movedLayout = layout.moveTo(new Point(315, 250));
 // Ensure that the first separators are moved:
 System.out.println(movedLayout.getVerticalSeparators().get(0)); // prints: 315
 System.out.println(movedLayout.getHorizontalSeparators().get(0)); // prints: 250
 Rectangle movedRect = movedLayout.getRectangle();
 // Prints: pos: (315, 250) size: (230, 75)
 System.out.println(String.format("pos: (%d, %d) size: (%d, %d)",
         movedRect.getLeft(), movedRect.getTop(),
         movedRect.getSize().getWidth(), movedRect.getSize().getHeight()));
 // movedLayout object is a copy of layout object, thus we can tune separators without the impact on the original layout:
 movedLayout.getHorizontalSeparators().add(90.0);
 System.out.println(movedLayout.getHorizontalSeparators().size()); // prints: 7
 System.out.println(layout.getHorizontalSeparators().size()); // prints: 6
 
````



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | point | [Point](../../com.groupdocs.parser.data/point) | नए लेआउट की स्थिति। |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new layout with the same size, separators and position in the point.

### scale(double factor) {#scale-double-}
```
public TemplateTableLayout scale(double factor)
```


दिए गए फ़ैक्टर द्वारा सभी निर्देशांक को स्केल करके इस लेआउट की एक कॉपी बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | फ़ैक्टर | double | स्केलिंग कारक। |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) with scaled separators.


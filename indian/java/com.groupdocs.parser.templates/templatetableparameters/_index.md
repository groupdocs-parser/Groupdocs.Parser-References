---
title: "TemplateTableParameters"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "तालिका पहचान एल्गोरिदम के लिए पैरामीटर प्रदान करता है।"
type: docs
weight: 22
url: /hi/java/com.groupdocs.parser.templates/templatetableparameters/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableParameters
```

तालिका पहचान एल्गोरिदम के लिए पैरामीटर प्रदान करता है।

टेबल का पता लगाने के लिए दो एल्गोरिदम हैं:

* Allows to detect a table in the rectangular area with set columns. This algorithm is useful for simple tables (without merged columns) and provides more accurate detection.
* Allows to detect a table in any place on the page. This is a more complex algorithm. It can detect tables in any place on the page. Additional parameters help to detect a table more correctly.

कुछ मामलों में जब एल्गोरिदम टेबल का पता नहीं लगा पाते या असटीक तरीके से करते हैं, तो [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) क्लास का उपयोग किया जाता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--) | नए [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
|
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-) | नए [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | टेबल को सम्मिलित करने वाले आयताकार क्षेत्र को प्राप्त करता है। |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | टेबल कॉलम विभाजकों को प्राप्त करता है। |
|
|  | [hasMergedCells()](#hasMergedCells--) | वह मान प्राप्त करता है जो दर्शाता है कि टेबल में मर्ज किए गए सेल हैं या नहीं। |
|
|  | [getMinRowCount()](#getMinRowCount--) | टेबल की न्यूनतम पंक्तियों की संख्या प्राप्त करता है। |
|
|  | [getMinColumnCount()](#getMinColumnCount--) | टेबल के न्यूनतम कॉलम की संख्या प्राप्त करता है। |
|
|  | [getMinVerticalSpace()](#getMinVerticalSpace--) | टेबल कॉलम के बीच न्यूनतम स्पेस प्राप्त करता है। |
|
|  | [scale(double factor)](#scale-double-) | इन पैरामीटरों की एक कॉपी बनाता है जिसमें सभी निर्देशांक दिए गए फैक्टर द्वारा स्केल किए गए हैं। |
|
### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)
```


नए [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | आयताकार क्षेत्र जो टेबल को समाहित करता है। |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | टेबल कॉलम विभाजक। |
|

### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)
```


नए [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | आयताकार क्षेत्र जो टेबल को समाहित करता है। |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | टेबल कॉलम विभाजक। |
|
|  | mergedCells | java.lang.Boolean | वह मान जो दर्शाता है कि टेबल में मर्ज किए गए सेल हैं या नहीं। |
|
|  | minRowCount | java.lang.Integer | टेबल पंक्तियों की न्यूनतम संख्या। |
|
|  | minColumnCount | java.lang.Integer | टेबल स्तंभों की न्यूनतम संख्या। |
|
|  | minVerticalSpace | java.lang.Integer | टेबल स्तंभों के बीच न्यूनतम अंतराल। |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


टेबल को सम्मिलित करने वाले आयताकार क्षेत्र को प्राप्त करता है।


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table;  null  if it isn't set.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


टेबल कॉलम विभाजकों को प्राप्त करता है।


**Returns:**
java.util.List<java.lang.Double> - डबल मानों का एक संग्रह जो टेबल स्तंभ विभाजकों के x-निर्देशांक को दर्शाता है;  null  यदि यह सेट नहीं है।

### hasMergedCells() {#hasMergedCells--}
```
public Boolean hasMergedCells()
```


वह मान प्राप्त करता है जो दर्शाता है कि टेबल में मर्ज किए गए सेल हैं या नहीं।


**Returns:**
java.lang.Boolean -  true  यदि टेबल में मर्ज्ड सेल्स हैं; अन्यथा,  false .  null  यदि यह सेट नहीं है।

### getMinRowCount() {#getMinRowCount--}
```
public Integer getMinRowCount()
```


टेबल की न्यूनतम पंक्तियों की संख्या प्राप्त करता है।


**Returns:**
java.lang.Integer - एक पूर्णांक मान जो टेबल पंक्तियों की न्यूनतम संख्या को दर्शाता है;  null  यदि यह सेट नहीं है।

### getMinColumnCount() {#getMinColumnCount--}
```
public Integer getMinColumnCount()
```


टेबल के न्यूनतम कॉलम की संख्या प्राप्त करता है।


**Returns:**
java.lang.Integer - एक पूर्णांक मान जो टेबल स्तंभों की न्यूनतम संख्या को दर्शाता है;  null  यदि यह सेट नहीं है।

### getMinVerticalSpace() {#getMinVerticalSpace--}
```
public Integer getMinVerticalSpace()
```


टेबल कॉलम के बीच न्यूनतम स्पेस प्राप्त करता है।


**Returns:**
java.lang.Integer - एक पूर्णांक मान जो टेबल स्तंभों के बीच न्यूनतम अंतराल को दर्शाता है;  null  यदि यह सेट नहीं है।

### scale(double factor) {#scale-double-}
```
public TemplateTableParameters scale(double factor)
```


इन पैरामीटरों की एक कॉपी बनाता है जिसमें सभी निर्देशांक दिए गए फैक्टर द्वारा स्केल किए गए हैं।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | फ़ैक्टर | double | स्केलिंग कारक। |
|

**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - A new [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) with scaled coordinates.


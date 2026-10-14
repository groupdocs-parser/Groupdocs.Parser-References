---
title: "TemplateRegexPosition"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "टेम्पलेट फ़ील्ड स्थिति प्रदान करता है जो नियमित अभिव्यक्ति का उपयोग करता है।"
type: docs
weight: 19
url: /hi/java/com.groupdocs.parser.templates/templateregexposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateRegexPosition extends TemplatePosition
```

टेम्पलेट फ़ील्ड स्थिति प्रदान करता है जो नियमित अभिव्यक्ति का उपयोग करता है।

निम्नलिखित उदाहरण दर्शाता है कि यदि दस्तावेज़ में "Invoice Number INV-12345" मौजूद है
फिर टेम्प्लेट फ़ील्ड को निम्नलिखित तरीके से परिभाषित किया जा सकता है:

````
// Create a regex template field with "InvoiceNumber" name
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+[A-Z0-9\\-]+"),
     "InvoiceNumber");
 
````

इस मामले में मान के रूप में पूरी स्ट्रिंग निकाली जाती है। स्ट्रिंग का केवल एक भाग निकालने के लिए
रेगुलर एक्सप्रेशन समूह "value" का उपयोग किया जाता है:

````
// Create a regex template field with "InvoiceNumber" name with "value" group
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+(?[A-Z0-9\\-]+)"),
     "InvoiceNumber");
````

इस मामले में मान के रूप में "INV-3337" स्ट्रिंग निकाली जाती है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [TemplateRegexPosition(String expression)](#TemplateRegexPosition-java.lang.String-) | नया उदाहरण प्रारंभ करता है [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition) क्लास का। |
|
|  | [TemplateRegexPosition(String expression, boolean matchCase)](#TemplateRegexPosition-java.lang.String-boolean-) | नया उदाहरण प्रारंभ करता है [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition) क्लास का। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getExpression()](#getExpression--) | नियमित अभिव्यक्ति प्राप्त करता है। |
|
|  | [isMatchCase()](#isMatchCase--) | उस मान को प्राप्त करता है जो दर्शाता है कि टेक्स्ट केस को अनदेखा नहीं किया गया है। |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateRegexPosition(String expression) {#TemplateRegexPosition-java.lang.String-}
```
public TemplateRegexPosition(String expression)
```


नया उदाहरण प्रारंभ करता है [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition) क्लास का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | expression | java.lang.String | नियमित अभिव्यक्ति। |
|

### TemplateRegexPosition(String expression, boolean matchCase) {#TemplateRegexPosition-java.lang.String-boolean-}
```
public TemplateRegexPosition(String expression, boolean matchCase)
```


नया उदाहरण प्रारंभ करता है [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition) क्लास का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | expression | java.lang.String | नियमित अभिव्यक्ति। |
|
|  | matchCase | boolean | वह मान जो दर्शाता है कि क्या टेक्स्ट केस को अनदेखा नहीं किया गया है। |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


नियमित अभिव्यक्ति प्राप्त करता है।


**Returns:**
java.lang.String - एक स्ट्रिंग जो नियमित अभिव्यक्ति को दर्शाती है।

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


उस मान को प्राप्त करता है जो दर्शाता है कि टेक्स्ट केस को अनदेखा नहीं किया गया है।


**Returns:**
boolean -  true  यदि टेक्स्ट केस को अनदेखा नहीं किया गया है; अन्यथा,  false .

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

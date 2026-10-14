---
title: "TemplateTable"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "टेम्प्लेट तालिका प्रदान करता है।"
type: docs
weight: 20
url: /hi/java/com.groupdocs.parser.templates/templatetable/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateTable extends TemplateItem
```

टेम्प्लेट तालिका प्रदान करता है।

टेबल को परिभाषित करने के दो तरीके हैं:

* Using [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class. In this case the table is defined by its position on the page: rectangular area, columns and rows separators.
* Using [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class. In this case the table is detected automatically by algorithms with set parameters. See [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class for more information.

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-) | [TemplateTable](../../com.groupdocs.parser.templates/templatetable) क्लास का नया उदाहरण बड़े अक्षरों वाले नाम के साथ आरंभ करता है। |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-) | [TemplateTable](../../com.groupdocs.parser.templates/templatetable) क्लास का नया उदाहरण बड़े अक्षरों वाले नाम के साथ आरंभ करता है। |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-) | एक नया उदाहरण प्रारंभ करता है [TemplateTable](../../com.groupdocs.parser.templates/templatetable) क्लास का। |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | एक नया उदाहरण प्रारंभ करता है [TemplateTable](../../com.groupdocs.parser.templates/templatetable) क्लास का। |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-) | [TemplateTable](../../com.groupdocs.parser.templates/templatetable) क्लास का नया उदाहरण बड़े अक्षरों वाले नाम के साथ आरंभ करता है। |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-) | एक नया उदाहरण प्रारंभ करता है [TemplateTable](../../com.groupdocs.parser.templates/templatetable) क्लास का। |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-) | एक नया उदाहरण प्रारंभ करता है [TemplateTable](../../com.groupdocs.parser.templates/templatetable) क्लास का। |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | एक नया उदाहरण प्रारंभ करता है [TemplateTable](../../com.groupdocs.parser.templates/templatetable) क्लास का। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getLayout()](#getLayout--) | टेबल लेआउट प्राप्त करता है। |
|
|  | [getParameters()](#getParameters--) | स्वचालित मोड में टेबल का पता लगाने के लिए पैरामीटर प्राप्त करता है। |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)
```


[TemplateTable](../../com.groupdocs.parser.templates/templatetable) क्लास का नया उदाहरण बड़े अक्षरों वाले नाम के साथ आरंभ करता है।

यदि टेबल स्वचालित रूप से पता नहीं चल सकती है तो टेम्पलेट टेबल को टेबल लेआउट द्वारा सेट किया जाता है:

````
TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 50.0, 95.0, 275.0 }),
     java.util.Arrays.asList(new Double[] { 325.0, 340.0, 365.0 }));
 TemplateTable table = new TemplateTable(layout, "Details", null);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
````



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | टेबल लेआउट। |
|
|  | नाम | java.lang.String | टेबल का नाम। |
|
|  | pageIndex | java.lang.Integer | पृष्ठ का इंडेक्स जहाँ टेम्पलेट टेबल स्थित है;  null  यदि टेम्पलेट टेबल किसी भी पृष्ठ पर स्थित है। |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)
```


[TemplateTable](../../com.groupdocs.parser.templates/templatetable) क्लास का नया उदाहरण बड़े अक्षरों वाले नाम के साथ आरंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | टेबल लेआउट। |
|
|  | नाम | java.lang.String | टेबल का नाम। |
|
|  | pageIndex | java.lang.Integer | पृष्ठ का इंडेक्स जहाँ टेम्पलेट टेबल स्थित है;  null  यदि टेम्पलेट टेबल किसी भी पृष्ठ पर स्थित है। |
|
|  | pageWidth | java.lang.Double | पृष्ठ की चौड़ाई जिसका उपयोग टेम्पलेट आइटम बनाने के लिए किया गया था। |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)
```


एक नया उदाहरण प्रारंभ करता है [TemplateTable](../../com.groupdocs.parser.templates/templatetable) क्लास का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | टेबल लेआउट। |
|
|  | नाम | java.lang.String | टेबल का नाम। |
|
|  | pageIndex | java.lang.Integer | पृष्ठ का इंडेक्स जहाँ टेम्पलेट टेबल स्थित है;  null  यदि टेम्पलेट टेबल किसी भी पृष्ठ पर स्थित है। |
|
|  | useUpperCaseName | boolean | वह मान जो दर्शाता है कि क्या नाम को UPPER CASE में परिवर्तित किया गया है। |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


एक नया उदाहरण प्रारंभ करता है [TemplateTable](../../com.groupdocs.parser.templates/templatetable) क्लास का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | टेबल लेआउट। |
|
|  | नाम | java.lang.String | टेबल का नाम। |
|
|  | pageIndex | java.lang.Integer | पृष्ठ का इंडेक्स जहाँ टेम्पलेट टेबल स्थित है;  null  यदि टेम्पलेट टेबल किसी भी पृष्ठ पर स्थित है। |
|
|  | pageWidth | java.lang.Double | पृष्ठ की चौड़ाई जिसका उपयोग टेम्पलेट आइटम बनाने के लिए किया गया था। |
|
|  | useUpperCaseName | boolean | वह मान जो दर्शाता है कि क्या नाम को UPPER CASE में परिवर्तित किया गया है। |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)
```


[TemplateTable](../../com.groupdocs.parser.templates/templatetable) क्लास का नया उदाहरण बड़े अक्षरों वाले नाम के साथ आरंभ करता है।

यदि टेम्पलेट टेबल डिटेक्टर पैरामीटर द्वारा सेट की गई है, तो टेबल स्वचालित रूप से पता लगाई जाती है:

````
TemplateTableParameters parameters = new TemplateTableParameters(
     new Rectangle(new Point(175, 350), new Size(400, 200)),
     java.util.Arrays.asList(new Double[] { 185.0, 370.0, 425.0, 485.0, 545.0 }));
 TemplateTable table = new TemplateTable(parameters, "Details", 0);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
 
````



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | स्वचालित मोड में टेबल का पता लगाने के लिए पैरामीटर। |
|
|  | नाम | java.lang.String | टेबल का नाम। |
|
|  | pageIndex | java.lang.Integer | पृष्ठ का इंडेक्स जहाँ टेम्पलेट टेबल स्थित है;  null  यदि टेम्पलेट टेबल किसी भी पृष्ठ पर स्थित है। |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)
```


एक नया उदाहरण प्रारंभ करता है [TemplateTable](../../com.groupdocs.parser.templates/templatetable) क्लास का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | स्वचालित मोड में टेबल का पता लगाने के लिए पैरामीटर। |
|
|  | नाम | java.lang.String | टेबल का नाम। |
|
|  | pageIndex | java.lang.Integer | पृष्ठ का इंडेक्स जहाँ टेम्पलेट टेबल स्थित है;  null  यदि टेम्पलेट टेबल किसी भी पृष्ठ पर स्थित है। |
|
|  | pageWidth | java.lang.Double | पृष्ठ की चौड़ाई जिसका उपयोग टेम्पलेट आइटम बनाने के लिए किया गया था। |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)
```


एक नया उदाहरण प्रारंभ करता है [TemplateTable](../../com.groupdocs.parser.templates/templatetable) क्लास का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | स्वचालित मोड में टेबल का पता लगाने के लिए पैरामीटर। |
|
|  | नाम | java.lang.String | टेबल का नाम। |
|
|  | pageIndex | java.lang.Integer | पृष्ठ का इंडेक्स जहाँ टेम्पलेट टेबल स्थित है;  null  यदि टेम्पलेट टेबल किसी भी पृष्ठ पर स्थित है। |
|
|  | useUpperCaseName | boolean | वह मान जो दर्शाता है कि क्या नाम को UPPER CASE में परिवर्तित किया गया है। |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


एक नया उदाहरण प्रारंभ करता है [TemplateTable](../../com.groupdocs.parser.templates/templatetable) क्लास का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | स्वचालित मोड में टेबल का पता लगाने के लिए पैरामीटर। |
|
|  | नाम | java.lang.String | टेबल का नाम। |
|
|  | pageIndex | java.lang.Integer | पृष्ठ का इंडेक्स जहाँ टेम्पलेट टेबल स्थित है;  null  यदि टेम्पलेट टेबल किसी भी पृष्ठ पर स्थित है। |
|
|  | pageWidth | java.lang.Double | पृष्ठ की चौड़ाई जिसका उपयोग टेम्पलेट आइटम बनाने के लिए किया गया था। |
|
|  | useUpperCaseName | boolean | वह मान जो दर्शाता है कि क्या नाम को UPPER CASE में परिवर्तित किया गया है। |
|

### getLayout() {#getLayout--}
```
public TemplateTableLayout getLayout()
```


टेबल लेआउट प्राप्त करता है।


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instance of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class that represents the table layout;  null  if it isn't set.

### getParameters() {#getParameters--}
```
public TemplateTableParameters getParameters()
```


स्वचालित मोड में टेबल का पता लगाने के लिए पैरामीटर प्राप्त करता है।


**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - An instance of  TemplateTableParameters  class that represents the parameters to detect the table in the automatic mode;  null  if it isn't set.

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

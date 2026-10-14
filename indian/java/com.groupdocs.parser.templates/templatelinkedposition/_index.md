---
title: "TemplateLinkedPosition"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "टेम्पलेट फ़ील्ड स्थिति प्रदान करता है जो लिंक्ड फ़ील्ड का उपयोग करता है।"
type: docs
weight: 15
url: /hi/java/com.groupdocs.parser.templates/templatelinkedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateLinkedPosition extends TemplatePosition
```

टेम्पलेट फ़ील्ड स्थिति प्रदान करता है जो लिंक्ड फ़ील्ड का उपयोग करता है।

निम्नलिखित उदाहरण कोड दिखाता है उस स्थिति के लिए यदि यह ज्ञात हो कि इनवॉइस नंबर वाला फ़ील्ड
\"Invoice number\" स्ट्रिंग के दाएँ स्थित है, निम्नलिखित कोड उपयोग किया जाता है:

````
// Create a regex template field to find "Invoice Number" text
 TemplateField invoice = new TemplateField(new TemplateRegexPosition("Invoice Number"), "Invoice");

 // Create a related template field associated with "Invoice" field and extract the value on the right of it
 TemplateField invoiceNumber = new TemplateField(
     new TemplateLinkedPosition("invoice", new Size(100, 15), new TemplateLinkedPositionEdges(false, false, true, false)),
     "InvoiceNumber");
 
````


## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-) | एक नया उदाहरण प्रारंभ करता है [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) क्लास का। |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-) | एक नया उदाहरण प्रारंभ करता है [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) क्लास का UPPER CASE नाम के साथ। |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-) | एक नया उदाहरण प्रारंभ करता है [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) क्लास का। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getLinkedFieldName()](#getLinkedFieldName--) | लिंक्ड फ़ील्ड का नाम प्राप्त करता है। |
|
|  | [getSearchArea()](#getSearchArea--) | उस क्षेत्र का आकार प्राप्त करता है जहाँ फ़ील्ड खोजा जाता है। |
|
|  | [isAutoScale()](#isAutoScale--) | वह मान प्राप्त करता है जो दर्शाता है कि क्या SearchArea को लिंक्ड फ़ील्ड आकार द्वारा स्केल किया गया है। |
|
|  | [getEdges()](#getEdges--) | लिंक्ड फ़ील्ड के किनारे प्राप्त करता है जहाँ फ़ील्ड खोजा जाता है। |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)
```


एक नया उदाहरण प्रारंभ करता है [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) क्लास का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | लिंक्ड फ़ील्ड का नाम। |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | फ़ील्ड खोजे जाने वाले क्षेत्र का आकार। |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | फ़ील्ड खोजे जाने वाले लिंक्ड फ़ील्ड के किनारे। |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)
```


एक नया उदाहरण प्रारंभ करता है [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) क्लास का UPPER CASE नाम के साथ।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | लिंक्ड फ़ील्ड का नाम। |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | फ़ील्ड खोजे जाने वाले क्षेत्र का आकार। |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | फ़ील्ड खोजे जाने वाले लिंक्ड फ़ील्ड के किनारे। |
|
|  | autoScale | boolean | यह मान दर्शाता है कि क्या searchArea को लिंक्ड फ़ील्ड के आकार द्वारा स्केल किया गया है। |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)
```


एक नया उदाहरण प्रारंभ करता है [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) क्लास का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | लिंक्ड फ़ील्ड का नाम। |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | फ़ील्ड खोजे जाने वाले क्षेत्र का आकार। |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | फ़ील्ड खोजे जाने वाले लिंक्ड फ़ील्ड के किनारे। |
|
|  | autoScale | boolean | यह मान दर्शाता है कि क्या searchArea को लिंक्ड फ़ील्ड के आकार द्वारा स्केल किया गया है.\\ |
|
|  | useUpperCaseName | boolean | वह मान जो दर्शाता है कि क्या नाम को UPPER CASE में परिवर्तित किया गया है। |
|

### getLinkedFieldName() {#getLinkedFieldName--}
```
public String getLinkedFieldName()
```


लिंक्ड फ़ील्ड का नाम प्राप्त करता है।


**Returns:**
java.lang.String - एक अपरकेस स्ट्रिंग मान जो लिंक्ड फ़ील्ड नाम का प्रतिनिधित्व करता है।

### getSearchArea() {#getSearchArea--}
```
public Size getSearchArea()
```


उस क्षेत्र का आकार प्राप्त करता है जहाँ फ़ील्ड खोजा जाता है।


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the area where a field is searched.

### isAutoScale() {#isAutoScale--}
```
public Boolean isAutoScale()
```


वह मान प्राप्त करता है जो दर्शाता है कि क्या SearchArea को लिंक्ड फ़ील्ड आकार द्वारा स्केल किया गया है।


**Returns:**
java.lang.Boolean - {code true} यदि  SearchArea  को लिंक्ड फ़ील्ड के आकार द्वारा स्केल किया गया है; अन्यथा,  false .

### getEdges() {#getEdges--}
```
public TemplateLinkedPositionEdges getEdges()
```


लिंक्ड फ़ील्ड के किनारे प्राप्त करता है जहाँ फ़ील्ड खोजा जाता है।


**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that represents the edges of the linked field where a field is searched.

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

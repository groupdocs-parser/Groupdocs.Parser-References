---
title: "TemplateLinkedPosition"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt een sjabloon-veldpositie die het gekoppelde veld gebruikt."
type: docs
weight: 15
url: /nl/java/com.groupdocs.parser.templates/templatelinkedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateLinkedPosition extends TemplatePosition
```

Biedt een sjabloon-veldpositie die het gekoppelde veld gebruikt.

Het volgende voorbeeld toont de code voor de situatie waarin bekend is dat het veld met een factuurnummer
aan de rechterkant van de string "Invoice number" staat, de volgende code wordt gebruikt:

````
// Create a regex template field to find "Invoice Number" text
 TemplateField invoice = new TemplateField(new TemplateRegexPosition("Invoice Number"), "Invoice");

 // Create a related template field associated with "Invoice" field and extract the value on the right of it
 TemplateField invoiceNumber = new TemplateField(
     new TemplateLinkedPosition("invoice", new Size(100, 15), new TemplateLinkedPositionEdges(false, false, true, false)),
     "InvoiceNumber");
 
````


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-) | Initialiseert een nieuw exemplaar van de [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) klasse. |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-) | Initialiseert een nieuw exemplaar van de [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) klasse met HOOFDLETTERS-naam. |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-) | Initialiseert een nieuw exemplaar van de [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getLinkedFieldName()](#getLinkedFieldName--) | Haalt de gekoppelde veldnaam op. |
|
|  | [getSearchArea()](#getSearchArea--) | Haalt de grootte van het gebied op waar een veld wordt gezocht. |
|
|  | [isAutoScale()](#isAutoScale--) | Haalt de waarde op die aangeeft of  SearchArea  wordt geschaald op basis van de grootte van het gekoppelde veld. |
|
|  | [getEdges()](#getEdges--) | Haalt de randen van het gekoppelde veld op waar een veld wordt gezocht. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)
```


Initialiseert een nieuw exemplaar van de [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | De naam van het gekoppelde veld. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | De grootte van het gebied waarin een veld wordt gezocht. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | De randen van het gekoppelde veld waarin een veld wordt gezocht. |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)
```


Initialiseert een nieuw exemplaar van de [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) klasse met HOOFDLETTERS-naam.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | De naam van het gekoppelde veld. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | De grootte van het gebied waarin een veld wordt gezocht. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | De randen van het gekoppelde veld waarin een veld wordt gezocht. |
|
|  | autoScale | boolean | De waarde die aangeeft of searchArea wordt geschaald op basis van de grootte van het gekoppelde veld. |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)
```


Initialiseert een nieuw exemplaar van de [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | De naam van het gekoppelde veld. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | De grootte van het gebied waarin een veld wordt gezocht. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | De randen van het gekoppelde veld waarin een veld wordt gezocht. |
|
|  | autoScale | boolean | De waarde die aangeeft of searchArea wordt geschaald op basis van de grootte van het gekoppelde veld.\\ |
|
|  | useUpperCaseName | boolean | De waarde die aangeeft of een  name  wordt geconverteerd naar HOOFDLETTERS. |
|

### getLinkedFieldName() {#getLinkedFieldName--}
```
public String getLinkedFieldName()
```


Haalt de gekoppelde veldnaam op.


**Returns:**
java.lang.String - Een hoofdlettergevoelige tekenreekswaarde die de naam van het gekoppelde veld weergeeft.

### getSearchArea() {#getSearchArea--}
```
public Size getSearchArea()
```


Haalt de grootte van het gebied op waar een veld wordt gezocht.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the area where a field is searched.

### isAutoScale() {#isAutoScale--}
```
public Boolean isAutoScale()
```


Haalt de waarde op die aangeeft of  SearchArea  wordt geschaald op basis van de grootte van het gekoppelde veld.


**Returns:**
java.lang.Boolean - {code true} als SearchArea wordt geschaald op basis van de grootte van het gekoppelde veld; anders false.

### getEdges() {#getEdges--}
```
public TemplateLinkedPositionEdges getEdges()
```


Haalt de randen van het gekoppelde veld op waar een veld wordt gezocht.


**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that represents the edges of the linked field where a field is searched.

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


Maakt een kopie van de huidige positie waarbij alle coördinaten worden geschaald met de opgegeven factor.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| factor | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)

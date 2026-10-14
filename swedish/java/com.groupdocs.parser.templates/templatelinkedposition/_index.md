---
title: "TemplateLinkedPosition"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller en mallfältposition som använder det länkade fältet."
type: docs
weight: 15
url: /sv/java/com.groupdocs.parser.templates/templatelinkedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateLinkedPosition extends TemplatePosition
```

Tillhandahåller en mallfältposition som använder det länkade fältet.

Följande exempel visar koden för situationen om det är känt att fältet med ett fakturanummer
är placerat till höger om strängen "Invoice number" används följande kod:

````
// Create a regex template field to find "Invoice Number" text
 TemplateField invoice = new TemplateField(new TemplateRegexPosition("Invoice Number"), "Invoice");

 // Create a related template field associated with "Invoice" field and extract the value on the right of it
 TemplateField invoiceNumber = new TemplateField(
     new TemplateLinkedPosition("invoice", new Size(100, 15), new TemplateLinkedPositionEdges(false, false, true, false)),
     "InvoiceNumber");
 
````


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-) | Initierar en ny instans av klassen [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition). |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-) | Initierar en ny instans av klassen [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) med namn i STORA BOKSTÄVER. |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-) | Initierar en ny instans av klassen [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getLinkedFieldName()](#getLinkedFieldName--) | Hämtar det länkade fältets namn. |
|
|  | [getSearchArea()](#getSearchArea--) | Hämtar storleken på området där ett fält söks. |
|
|  | [isAutoScale()](#isAutoScale--) | Hämtar värdet som indikerar om  SearchArea  skalas efter den länkade fältets storlek. |
|
|  | [getEdges()](#getEdges--) | Hämtar kanterna på det länkade fältet där ett fält söks. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)
```


Initierar en ny instans av klassen [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | Namnet på det länkade fältet. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | Storleken på området där ett fält söks. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | Kanterna på det länkade fältet där ett fält söks. |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)
```


Initierar en ny instans av klassen [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) med namn i STORA BOKSTÄVER.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | Namnet på det länkade fältet. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | Storleken på området där ett fält söks. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | Kanterna på det länkade fältet där ett fält söks. |
|
|  | autoScale | boolean | Värdet som indikerar om searchArea skalas efter den länkade fältets storlek. |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)
```


Initierar en ny instans av klassen [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | Namnet på det länkade fältet. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | Storleken på området där ett fält söks. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | Kanterna på det länkade fältet där ett fält söks. |
|
|  | autoScale | boolean | Värdet som indikerar om searchArea skalas efter den länkade fältets storlek.\\ |
|
|  | useUpperCaseName | boolean | Värdet som indikerar om ett  name  konverteras till STORA BOKSTÄVER. |
|

### getLinkedFieldName() {#getLinkedFieldName--}
```
public String getLinkedFieldName()
```


Hämtar det länkade fältets namn.


**Returns:**
java.lang.String - Ett strängvärde i stora bokstäver som representerar det länkade fältets namn.

### getSearchArea() {#getSearchArea--}
```
public Size getSearchArea()
```


Hämtar storleken på området där ett fält söks.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the area where a field is searched.

### isAutoScale() {#isAutoScale--}
```
public Boolean isAutoScale()
```


Hämtar värdet som indikerar om  SearchArea  skalas efter den länkade fältets storlek.


**Returns:**
java.lang.Boolean - {code true} om  SearchArea  skalas efter den länkade fältets storlek; annars  false .

### getEdges() {#getEdges--}
```
public TemplateLinkedPositionEdges getEdges()
```


Hämtar kanterna på det länkade fältet där ett fält söks.


**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that represents the edges of the linked field where a field is searched.

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


Skapar en kopia av den aktuella positionen med alla koordinater skalade med den angivna faktorn.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| faktor | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)

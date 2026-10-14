---
title: "TemplateLinkedPosition"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt eine Vorlagenfeldposition bereit, die das verknüpfte Feld verwendet."
type: docs
weight: 15
url: /de/java/com.groupdocs.parser.templates/templatelinkedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateLinkedPosition extends TemplatePosition
```

Stellt eine Vorlagenfeldposition bereit, die das verknüpfte Feld verwendet.

Das folgende Beispiel zeigt den Code für den Fall, dass bekannt ist, dass das Feld mit einer Rechnungsnummer
rechts vom String "Invoice number" platziert ist, wird folgender Code verwendet:

````
// Create a regex template field to find "Invoice Number" text
 TemplateField invoice = new TemplateField(new TemplateRegexPosition("Invoice Number"), "Invoice");

 // Create a related template field associated with "Invoice" field and extract the value on the right of it
 TemplateField invoiceNumber = new TemplateField(
     new TemplateLinkedPosition("invoice", new Size(100, 15), new TemplateLinkedPositionEdges(false, false, true, false)),
     "InvoiceNumber");
 
````


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-) | Initialisiert eine neue Instanz der Klasse [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition). |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-) | Initialisiert eine neue Instanz der Klasse [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) mit einem GROSSBUCHSTABEN-Namen. |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-) | Initialisiert eine neue Instanz der Klasse [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getLinkedFieldName()](#getLinkedFieldName--) | Liefert den Namen des verknüpften Feldes. |
|
|  | [getSearchArea()](#getSearchArea--) | Liefert die Größe des Bereichs, in dem ein Feld gesucht wird. |
|
|  | [isAutoScale()](#isAutoScale--) | Liefert den Wert, der angibt, ob  SearchArea  anhand der Größe des verknüpften Feldes skaliert wird. |
|
|  | [getEdges()](#getEdges--) | Liefert die Kanten des verknüpften Feldes, in dem ein Feld gesucht wird. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)
```


Initialisiert eine neue Instanz der Klasse [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | Der Name des verknüpften Feldes. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | Die Größe des Bereichs, in dem ein Feld gesucht wird. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | Die Kanten des verknüpften Feldes, in dem ein Feld gesucht wird. |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)
```


Initialisiert eine neue Instanz der Klasse [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) mit einem GROSSBUCHSTABEN-Namen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | Der Name des verknüpften Feldes. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | Die Größe des Bereichs, in dem ein Feld gesucht wird. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | Die Kanten des verknüpften Feldes, in dem ein Feld gesucht wird. |
|
|  | autoScale | boolean | Der Wert, der angibt, ob searchArea anhand der Größe des verknüpften Feldes skaliert wird. |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)
```


Initialisiert eine neue Instanz der Klasse [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | Der Name des verknüpften Feldes. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | Die Größe des Bereichs, in dem ein Feld gesucht wird. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | Die Kanten des verknüpften Feldes, in dem ein Feld gesucht wird. |
|
|  | autoScale | boolean | Der Wert, der angibt, ob searchArea anhand der Größe des verknüpften Feldes skaliert wird.\\ |
|
|  | useUpperCaseName | boolean | Der Wert, der angibt, ob ein  Name  in GROSSBUCHSTABEN umgewandelt wird. |
|

### getLinkedFieldName() {#getLinkedFieldName--}
```
public String getLinkedFieldName()
```


Liefert den Namen des verknüpften Feldes.


**Returns:**
java.lang.String - Ein Großbuchstaben-Stringwert, der den Namen des verknüpften Feldes darstellt.

### getSearchArea() {#getSearchArea--}
```
public Size getSearchArea()
```


Liefert die Größe des Bereichs, in dem ein Feld gesucht wird.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the area where a field is searched.

### isAutoScale() {#isAutoScale--}
```
public Boolean isAutoScale()
```


Liefert den Wert, der angibt, ob  SearchArea  anhand der Größe des verknüpften Feldes skaliert wird.


**Returns:**
java.lang.Boolean - {code true} wenn  SearchArea  anhand der Größe des verknüpften Feldes skaliert wird; andernfalls  false .

### getEdges() {#getEdges--}
```
public TemplateLinkedPositionEdges getEdges()
```


Liefert die Kanten des verknüpften Feldes, in dem ein Feld gesucht wird.


**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that represents the edges of the linked field where a field is searched.

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


Erstellt eine Kopie der aktuellen Position, wobei alle Koordinaten um den angegebenen Faktor skaliert werden.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Faktor | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)

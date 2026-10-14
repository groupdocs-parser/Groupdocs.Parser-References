---
title: "TemplateLinkedPosition"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit une position de champ de modèle qui utilise le champ lié."
type: docs
weight: 15
url: /fr/java/com.groupdocs.parser.templates/templatelinkedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateLinkedPosition extends TemplatePosition
```

Fournit une position de champ de modèle qui utilise le champ lié.

L'exemple suivant montre le code pour le cas où il est connu que le champ contenant un numéro de facture
est placé à droite de la chaîne "Invoice number" le code suivant est utilisé :

````
// Create a regex template field to find "Invoice Number" text
 TemplateField invoice = new TemplateField(new TemplateRegexPosition("Invoice Number"), "Invoice");

 // Create a related template field associated with "Invoice" field and extract the value on the right of it
 TemplateField invoiceNumber = new TemplateField(
     new TemplateLinkedPosition("invoice", new Size(100, 15), new TemplateLinkedPositionEdges(false, false, true, false)),
     "InvoiceNumber");
 
````


## Constructors

| Constructor | Description |
| --- | --- |
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-) | Initialise une nouvelle instance de la classe [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition). |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-) | Initialise une nouvelle instance de la classe [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) avec le nom en MAJUSCULE. |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-) | Initialise une nouvelle instance de la classe [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getLinkedFieldName()](#getLinkedFieldName--) | Obtient le nom du champ lié. |
|
|  | [getSearchArea()](#getSearchArea--) | Obtient la taille de la zone où un champ est recherché. |
|
|  | [isAutoScale()](#isAutoScale--) | Obtient la valeur qui indique si  SearchArea  est mise à l'échelle par la taille du champ lié. |
|
|  | [getEdges()](#getEdges--) | Obtient les bords du champ lié où un champ est recherché. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)
```


Initialise une nouvelle instance de la classe [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | Le nom du champ lié. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | La taille de la zone où un champ est recherché. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | Les bords du champ lié où un champ est recherché. |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)
```


Initialise une nouvelle instance de la classe [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) avec le nom en MAJUSCULE.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | Le nom du champ lié. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | La taille de la zone où un champ est recherché. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | Les bords du champ lié où un champ est recherché. |
|
|  | autoScale | boolean | La valeur qui indique si searchArea est mise à l'échelle par la taille du champ lié. |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)
```


Initialise une nouvelle instance de la classe [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | Le nom du champ lié. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | La taille de la zone où un champ est recherché. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | Les bords du champ lié où un champ est recherché. |
|
|  | autoScale | boolean | La valeur qui indique si searchArea est mise à l'échelle par la taille du champ lié.\\ |
|
|  | useUpperCaseName | boolean | La valeur qui indique si un  name  est converti en MAJUSCULE. |
|

### getLinkedFieldName() {#getLinkedFieldName--}
```
public String getLinkedFieldName()
```


Obtient le nom du champ lié.


**Returns:**
java.lang.String - Une valeur de chaîne en majuscules qui représente le nom du champ lié.

### getSearchArea() {#getSearchArea--}
```
public Size getSearchArea()
```


Obtient la taille de la zone où un champ est recherché.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the area where a field is searched.

### isAutoScale() {#isAutoScale--}
```
public Boolean isAutoScale()
```


Obtient la valeur qui indique si  SearchArea  est mise à l'échelle par la taille du champ lié.


**Returns:**
java.lang.Boolean - {code true} si  SearchArea  est mise à l'échelle par la taille du champ lié ; sinon,  false .

### getEdges() {#getEdges--}
```
public TemplateLinkedPositionEdges getEdges()
```


Obtient les bords du champ lié où un champ est recherché.


**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that represents the edges of the linked field where a field is searched.

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


Crée une copie de la position actuelle avec toutes les coordonnées mises à l'échelle par le facteur donné.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| factor | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)

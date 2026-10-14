---
title: "TemplateLinkedPositionEdges"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit les bords du champ lié où le champ de texte est recherché."
type: docs
weight: 16
url: /fr/java/com.groupdocs.parser.templates/templatelinkedpositionedges/
---
**Inheritance:**
java.lang.Object
```
public class TemplateLinkedPositionEdges
```

Fournit les bords du champ lié où le champ texte est recherché. [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) est utilisé dans la classe [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).

## Constructors

| Constructor | Description |
| --- | --- |
|  | [TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)](#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-) | Initialise une nouvelle instance de la classe [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [isEmpty()](#isEmpty--) | Obtient la valeur qui indique si l'instance est vide. |
|
|  | [isLeft()](#isLeft--) | Obtient la valeur qui indique si un champ est recherché par la gauche du champ lié. |
|
|  | [isTop()](#isTop--) | Obtient la valeur qui indique si un champ est recherché par le haut du champ lié. |
|
|  | [isRight()](#isRight--) | Obtient la valeur qui indique si un champ est recherché par la droite du champ lié. |
|
|  | [isBottom()](#isBottom--) | Obtient la valeur qui indique si un champ est recherché par le bas du champ lié. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Convertit la représentation sous forme de chaîne des bords en son équivalent de classe. |
|
| [toString()](#toString--) |  |
### TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom) {#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-}
```
public TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)
```


Initialise une nouvelle instance de la classe [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | gauche | boolean | La valeur qui indique si un champ est recherché par la gauche à partir du champ lié. |
|
|  | haut | boolean | La valeur qui indique si un champ est recherché par le haut à partir du champ lié. |
|
|  | droite | boolean | La valeur qui indique si un champ est recherché par la droite à partir du champ lié. |
|
|  | bas | boolean | La valeur qui indique si un champ est recherché par le bas à partir du champ lié. |
|

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Obtient la valeur qui indique si l'instance est vide.


**Returns:**
booléen -  true  si l'instance est vide (tous les champs sont  false ); sinon,  false .

### isLeft() {#isLeft--}
```
public boolean isLeft()
```


Obtient la valeur qui indique si un champ est recherché par la gauche du champ lié.


**Returns:**
booléen -  true  si un champ est recherché par la gauche à partir du champ lié ; sinon,  false .

### isTop() {#isTop--}
```
public boolean isTop()
```


Obtient la valeur qui indique si un champ est recherché par le haut du champ lié.


**Returns:**
booléen -  true  si un champ est recherché par le haut à partir du champ lié ; sinon,  false .

### isRight() {#isRight--}
```
public boolean isRight()
```


Obtient la valeur qui indique si un champ est recherché par la droite du champ lié.


**Returns:**
booléen -  true  si un champ est recherché par la droite à partir du champ lié ; sinon,  false .

### isBottom() {#isBottom--}
```
public boolean isBottom()
```


Obtient la valeur qui indique si un champ est recherché par le bas du champ lié.


**Returns:**
booléen -  true  si un champ est recherché par le bas à partir du champ lié ; sinon,  false .

### parse(String s) {#parse-java.lang.String-}
```
public static TemplateLinkedPositionEdges parse(String s)
```


Convertit la représentation sous forme de chaîne des bords en son équivalent de classe.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | s | java.lang.String | Une chaîne qui contient les bords à convertir. |
|

**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String

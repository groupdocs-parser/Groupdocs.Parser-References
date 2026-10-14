---
title: "TemplateLinkedPositionEdges"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Kanten des verknüpften Feldes bereit, in denen das Textfeld gesucht wird."
type: docs
weight: 16
url: /de/java/com.groupdocs.parser.templates/templatelinkedpositionedges/
---
**Inheritance:**
java.lang.Object
```
public class TemplateLinkedPositionEdges
```

Stellt die Kanten des verknüpften Feldes bereit, in dem das Textfeld gesucht wird. [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) wird in der Klasse [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) verwendet.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)](#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-) | Initialisiert eine neue Instanz der Klasse [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [isEmpty()](#isEmpty--) | Gibt den Wert zurück, der angibt, ob die Instanz leer ist. |
|
|  | [isLeft()](#isLeft--) | Gibt den Wert zurück, der angibt, ob ein Feld von links aus dem verknüpften Feld aus gesucht wird. |
|
|  | [isTop()](#isTop--) | Gibt den Wert zurück, der angibt, ob ein Feld von oben aus dem verknüpften Feld aus gesucht wird. |
|
|  | [isRight()](#isRight--) | Gibt den Wert zurück, der angibt, ob ein Feld von rechts aus dem verknüpften Feld aus gesucht wird. |
|
|  | [isBottom()](#isBottom--) | Gibt den Wert zurück, der angibt, ob ein Feld von unten aus dem verknüpften Feld aus gesucht wird. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Konvertiert die Zeichenkettenrepräsentation der Kanten in das entsprechende Klassenobjekt. |
|
| [toString()](#toString--) |  |
### TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom) {#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-}
```
public TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)
```


Initialisiert eine neue Instanz der Klasse [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | links | boolean | Der Wert, der angibt, ob ein Feld von links aus dem verknüpften Feld aus gesucht wird. |
|
|  | oben | boolean | Der Wert, der angibt, ob ein Feld von oben aus dem verknüpften Feld aus gesucht wird. |
|
|  | rechts | boolean | Der Wert, der angibt, ob ein Feld von rechts aus dem verknüpften Feld aus gesucht wird. |
|
|  | unten | boolean | Der Wert, der angibt, ob ein Feld von unten aus dem verknüpften Feld aus gesucht wird. |
|

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Gibt den Wert zurück, der angibt, ob die Instanz leer ist.


**Returns:**
boolean -  true  wenn die Instanz leer ist (alle Felder sind  false ); andernfalls,  false .

### isLeft() {#isLeft--}
```
public boolean isLeft()
```


Gibt den Wert zurück, der angibt, ob ein Feld von links aus dem verknüpften Feld aus gesucht wird.


**Returns:**
boolean -  true  wenn ein Feld von links aus dem verknüpften Feld aus gesucht wird; andernfalls,  false .

### isTop() {#isTop--}
```
public boolean isTop()
```


Gibt den Wert zurück, der angibt, ob ein Feld von oben aus dem verknüpften Feld aus gesucht wird.


**Returns:**
boolean -  true  wenn ein Feld von oben aus dem verknüpften Feld aus gesucht wird; andernfalls,  false .

### isRight() {#isRight--}
```
public boolean isRight()
```


Gibt den Wert zurück, der angibt, ob ein Feld von rechts aus dem verknüpften Feld aus gesucht wird.


**Returns:**
boolean -  true  wenn ein Feld von rechts aus dem verknüpften Feld aus gesucht wird; andernfalls,  false .

### isBottom() {#isBottom--}
```
public boolean isBottom()
```


Gibt den Wert zurück, der angibt, ob ein Feld von unten aus dem verknüpften Feld aus gesucht wird.


**Returns:**
boolean -  true  wenn ein Feld von unten aus dem verknüpften Feld aus gesucht wird; andernfalls,  false .

### parse(String s) {#parse-java.lang.String-}
```
public static TemplateLinkedPositionEdges parse(String s)
```


Konvertiert die Zeichenkettenrepräsentation der Kanten in das entsprechende Klassenobjekt.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | s | java.lang.String | Eine Zeichenkette, die Kanten zum Konvertieren enthält. |
|

**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String

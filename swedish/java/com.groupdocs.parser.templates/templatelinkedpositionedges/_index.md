---
title: "TemplateLinkedPositionEdges"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller kanterna på det länkade fältet där textfältet söks."
type: docs
weight: 16
url: /sv/java/com.groupdocs.parser.templates/templatelinkedpositionedges/
---
**Inheritance:**
java.lang.Object
```
public class TemplateLinkedPositionEdges
```

Tillhandahåller kanterna på det länkade fältet där textfältet söks. [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) används i klassen [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)](#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-) | Initierar en ny instans av klassen [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [isEmpty()](#isEmpty--) | Hämtar värdet som indikerar om instansen är tom. |
|
|  | [isLeft()](#isLeft--) | Hämtar värdet som indikerar om ett fält söks från vänster av det länkade fältet. |
|
|  | [isTop()](#isTop--) | Hämtar värdet som indikerar om ett fält söks från toppen av det länkade fältet. |
|
|  | [isRight()](#isRight--) | Hämtar värdet som indikerar om ett fält söks från höger från det länkade fältet. |
|
|  | [isBottom()](#isBottom--) | Hämtar värdet som indikerar om ett fält söks från botten från det länkade fältet. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Konverterar strängrepresentationen av kanter till dess klassmotsvarighet. |
|
| [toString()](#toString--) |  |
### TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom) {#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-}
```
public TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)
```


Initierar en ny instans av klassen [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | vänster | boolean | Värdet som indikerar om ett fält söks från vänster från det länkade fältet. |
|
|  | övre | boolean | Värdet som indikerar om ett fält söks från övre från det länkade fältet. |
|
|  | höger | boolean | Värdet som indikerar om ett fält söks från höger från det länkade fältet. |
|
|  | botten | boolean | Värdet som indikerar om ett fält söks från botten från det länkade fältet. |
|

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Hämtar värdet som indikerar om instansen är tom.


**Returns:**
boolean -  true  om instansen är tom (alla fält är  false ); annars,  false .

### isLeft() {#isLeft--}
```
public boolean isLeft()
```


Hämtar värdet som indikerar om ett fält söks från vänster av det länkade fältet.


**Returns:**
boolean -  true  om ett fält söks från vänster från det länkade fältet; annars,  false .

### isTop() {#isTop--}
```
public boolean isTop()
```


Hämtar värdet som indikerar om ett fält söks från toppen av det länkade fältet.


**Returns:**
boolean -  true  om ett fält söks från övre från det länkade fältet; annars,  false .

### isRight() {#isRight--}
```
public boolean isRight()
```


Hämtar värdet som indikerar om ett fält söks från höger från det länkade fältet.


**Returns:**
boolean -  true  om ett fält söks från höger från det länkade fältet; annars,  false .

### isBottom() {#isBottom--}
```
public boolean isBottom()
```


Hämtar värdet som indikerar om ett fält söks från botten från det länkade fältet.


**Returns:**
boolean -  true  om ett fält söks från botten från det länkade fältet; annars,  false .

### parse(String s) {#parse-java.lang.String-}
```
public static TemplateLinkedPositionEdges parse(String s)
```


Konverterar strängrepresentationen av kanter till dess klassmotsvarighet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | s | java.lang.String | En sträng som innehåller kanter att konvertera. |
|

**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String

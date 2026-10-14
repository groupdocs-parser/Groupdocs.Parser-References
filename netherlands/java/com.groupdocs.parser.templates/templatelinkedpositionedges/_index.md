---
title: "TemplateLinkedPositionEdges"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt de randen van het gekoppelde veld waar het tekstveld wordt gezocht."
type: docs
weight: 16
url: /nl/java/com.groupdocs.parser.templates/templatelinkedpositionedges/
---
**Inheritance:**
java.lang.Object
```
public class TemplateLinkedPositionEdges
```

Biedt de randen van het gekoppelde veld waar het tekstveld wordt gezocht. [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) wordt gebruikt in de [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) klasse.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)](#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-) | Initialiseert een nieuw exemplaar van de [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [isEmpty()](#isEmpty--) | Haalt de waarde op die aangeeft of het exemplaar leeg is. |
|
|  | [isLeft()](#isLeft--) | Haalt de waarde op die aangeeft of een veld vanaf links van het gekoppelde veld wordt gezocht. |
|
|  | [isTop()](#isTop--) | Haalt de waarde op die aangeeft of een veld vanaf boven van het gekoppelde veld wordt gezocht. |
|
|  | [isRight()](#isRight--) | Haalt de waarde op die aangeeft of een veld vanaf rechts van het gekoppelde veld wordt gezocht. |
|
|  | [isBottom()](#isBottom--) | Haalt de waarde op die aangeeft of een veld vanaf onder van het gekoppelde veld wordt gezocht. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Converteert de tekenreeksrepresentatie van randen naar de equivalente klasse. |
|
| [toString()](#toString--) |  |
### TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom) {#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-}
```
public TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)
```


Initialiseert een nieuw exemplaar van de [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | left | boolean | De waarde die aangeeft of een veld vanaf links van het gekoppelde veld wordt gezocht. |
|
|  | top | boolean | De waarde die aangeeft of een veld vanaf boven van het gekoppelde veld wordt gezocht. |
|
|  | rechts | boolean | De waarde die aangeeft of een veld wordt doorzocht vanaf rechts van het gekoppelde veld. |
|
|  | onder | boolean | De waarde die aangeeft of een veld wordt doorzocht vanaf onder het gekoppelde veld. |
|

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Haalt de waarde op die aangeeft of het exemplaar leeg is.


**Returns:**
boolean -  true  als de instantie leeg is (alle velden zijn  false ); anders,  false .

### isLeft() {#isLeft--}
```
public boolean isLeft()
```


Haalt de waarde op die aangeeft of een veld vanaf links van het gekoppelde veld wordt gezocht.


**Returns:**
boolean -  true  als een veld wordt doorzocht vanaf links van het gekoppelde veld; anders,  false .

### isTop() {#isTop--}
```
public boolean isTop()
```


Haalt de waarde op die aangeeft of een veld vanaf boven van het gekoppelde veld wordt gezocht.


**Returns:**
boolean -  true  als een veld wordt doorzocht vanaf boven van het gekoppelde veld; anders,  false .

### isRight() {#isRight--}
```
public boolean isRight()
```


Haalt de waarde op die aangeeft of een veld vanaf rechts van het gekoppelde veld wordt gezocht.


**Returns:**
boolean -  true  als een veld wordt doorzocht vanaf rechts van het gekoppelde veld; anders,  false .

### isBottom() {#isBottom--}
```
public boolean isBottom()
```


Haalt de waarde op die aangeeft of een veld vanaf onder van het gekoppelde veld wordt gezocht.


**Returns:**
boolean -  true  als een veld wordt doorzocht vanaf onder van het gekoppelde veld; anders,  false .

### parse(String s) {#parse-java.lang.String-}
```
public static TemplateLinkedPositionEdges parse(String s)
```


Converteert de tekenreeksrepresentatie van randen naar de equivalente klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | s | java.lang.String | Een tekenreeks die randen bevat om te converteren. |
|

**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String

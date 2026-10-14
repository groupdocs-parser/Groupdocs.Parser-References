---
title: "TemplateField"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt das Vorlagen-Textfeld bereit."
type: docs
weight: 12
url: /de/java/com.groupdocs.parser.templates/templatefield/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateField extends TemplateItem
```

Stellt das Vorlagen-Textfeld bereit.

Textfelder werden durch ihre Position auf der Seite definiert. Es gibt drei Möglichkeiten, ein Textfeld zu definieren:

* Using the rectangular area: [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition)
* Using the regular expression: [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition)
* Using the linked field: [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [TemplateField(TemplatePosition position, String name)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [TemplateField](../../com.groupdocs.parser.templates/templatefield). |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-) | Initialisiert eine neue Instanz der Klasse [TemplateField](../../com.groupdocs.parser.templates/templatefield) mit dem GROSSBUCHSTABEN-Namen. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-) | Initialisiert eine neue Instanz der Klasse [TemplateField](../../com.groupdocs.parser.templates/templatefield) mit dem GROSSBUCHSTABEN-Namen. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-) | Initialisiert eine neue Instanz der Klasse [TemplateField](../../com.groupdocs.parser.templates/templatefield). |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Initialisiert eine neue Instanz der Klasse [TemplateField](../../com.groupdocs.parser.templates/templatefield). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getPosition()](#getPosition--) | Liefert den Wert, der beschreibt, wie das Vorlagenfeld auf der Dokumentenseite gefunden wird. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateField(TemplatePosition position, String name) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-}
```
public TemplateField(TemplatePosition position, String name)
```


Initialisiert eine neue Instanz der Klasse [TemplateField](../../com.groupdocs.parser.templates/templatefield).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Die Feldposition. |
|
|  | Name | java.lang.String | Der Feldname. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex)
```


Initialisiert eine neue Instanz der Klasse [TemplateField](../../com.groupdocs.parser.templates/templatefield) mit dem GROSSBUCHSTABEN-Namen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Die Feldposition. |
|
|  | Name | java.lang.String | Der Feldname. |
|
|  | pageIndex | java.lang.Integer | Ein ganzzahliger Wert, der den Index der Seite darstellt, auf der das Vorlagenelement gefunden wird;  null  falls das Vorlagenelement auf einer beliebigen Seite liegt. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)
```


Initialisiert eine neue Instanz der Klasse [TemplateField](../../com.groupdocs.parser.templates/templatefield) mit dem GROSSBUCHSTABEN-Namen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Die Feldposition. |
|
|  | Name | java.lang.String | Der Feldname. |
|
|  | pageIndex | java.lang.Integer | Ein ganzzahliger Wert, der den Index der Seite darstellt, auf der das Vorlagenelement gefunden wird;  null  falls das Vorlagenelement auf einer beliebigen Seite liegt. |
|
|  | pageWidth | java.lang.Double | Die Breite der Seite, die zur Erstellung des Vorlagen-Elements verwendet wurde. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)
```


Initialisiert eine neue Instanz der Klasse [TemplateField](../../com.groupdocs.parser.templates/templatefield).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Die Feldposition. |
|
|  | Name | java.lang.String | Der Feldname. |
|
|  | pageIndex | java.lang.Integer | Ein ganzzahliger Wert, der den Index der Seite darstellt, auf der das Vorlagenelement gefunden wird;  null  falls das Vorlagenelement auf einer beliebigen Seite liegt. |
|
|  | useUpperCaseName | boolean | Der Wert, der angibt, ob ein  Name  in GROSSBUCHSTABEN umgewandelt wird. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Initialisiert eine neue Instanz der Klasse [TemplateField](../../com.groupdocs.parser.templates/templatefield).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Die Feldposition. |
|
|  | Name | java.lang.String | Der Feldname. |
|
|  | pageIndex | java.lang.Integer | Ein ganzzahliger Wert, der den Index der Seite darstellt, auf der das Vorlagenelement gefunden wird;  null  falls das Vorlagenelement auf einer beliebigen Seite liegt. |
|
|  | pageWidth | java.lang.Double | Die Breite der Seite, die zur Erstellung des Vorlagen-Elements verwendet wurde. |
|
|  | useUpperCaseName | boolean | Der Wert, der angibt, ob ein  Name  in GROSSBUCHSTABEN umgewandelt wird. |
|

### getPosition() {#getPosition--}
```
public TemplatePosition getPosition()
```


Liefert den Wert, der beschreibt, wie das Vorlagenfeld auf der Dokumentenseite gefunden wird.


**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - An instance of [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) descendant class.

### scale(double factor) {#scale-double-}
```
public TemplateItem scale(double factor)
```


Erstellt eine Kopie des aktuellen Elements, wobei alle Koordinaten um den angegebenen Faktor skaliert werden.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Faktor | double |  |

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem)

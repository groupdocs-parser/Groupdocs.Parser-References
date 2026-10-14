---
title: "TemplateTableParameters"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt Parameter für die Tabellenerkennungs‑Algorithmen bereit."
type: docs
weight: 22
url: /de/java/com.groupdocs.parser.templates/templatetableparameters/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableParameters
```

Stellt Parameter für die Tabellenerkennungs‑Algorithmen bereit.

Es gibt zwei Algorithmen, um eine Tabelle zu erkennen:

* Allows to detect a table in the rectangular area with set columns. This algorithm is useful for simple tables (without merged columns) and provides more accurate detection.
* Allows to detect a table in any place on the page. This is a more complex algorithm. It can detect tables in any place on the page. Additional parameters help to detect a table more correctly.

In einigen Fällen, wenn Algorithmen eine Tabelle nicht erkennen können oder dies ungenau tun, wird die Klasse [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) verwendet.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--) | Initialisiert eine neue Instanz der Klasse [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters). |
|
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-) | Initialisiert eine neue Instanz der Klasse [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Gibt den rechteckigen Bereich zurück, der die Tabelle enthält. |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | Gibt die Trennlinien der Tabellenspalten zurück. |
|
|  | [hasMergedCells()](#hasMergedCells--) | Liefert den Wert, der angibt, ob die Tabelle zusammengeführte Zellen hat. |
|
|  | [getMinRowCount()](#getMinRowCount--) | Liefert die minimale Anzahl der Tabellenzeilen. |
|
|  | [getMinColumnCount()](#getMinColumnCount--) | Liefert die minimale Anzahl der Tabellenspalten. |
|
|  | [getMinVerticalSpace()](#getMinVerticalSpace--) | Liefert den minimalen Abstand zwischen den Tabellenspalten. |
|
|  | [scale(double factor)](#scale-double-) | Erstellt eine Kopie dieser Parameter, wobei alle Koordinaten um den angegebenen Faktor skaliert werden. |
|
### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)
```


Initialisiert eine neue Instanz der Klasse [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Der rechteckige Bereich, der die Tabelle enthält. |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | Die Trennlinien der Tabellenspalten. |
|

### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)
```


Initialisiert eine neue Instanz der Klasse [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Der rechteckige Bereich, der die Tabelle enthält. |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | Die Trennlinien der Tabellenspalten. |
|
|  | mergedCells | java.lang.Boolean | Der Wert, der angibt, ob die Tabelle zusammengeführte Zellen hat. |
|
|  | minRowCount | java.lang.Integer | Die minimale Anzahl der Tabellenzeilen. |
|
|  | minColumnCount | java.lang.Integer | Die minimale Anzahl der Tabellenspalten. |
|
|  | minVerticalSpace | java.lang.Integer | Der minimale Abstand zwischen den Tabellenspalten. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Gibt den rechteckigen Bereich zurück, der die Tabelle enthält.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table;  null  if it isn't set.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


Gibt die Trennlinien der Tabellenspalten zurück.


**Returns:**
java.util.List<java.lang.Double> - Eine Sammlung von Double-Werten, die die x-Koordinaten der Trennlinien der Tabellenspalten darstellen;  null  wenn sie nicht gesetzt ist.

### hasMergedCells() {#hasMergedCells--}
```
public Boolean hasMergedCells()
```


Liefert den Wert, der angibt, ob die Tabelle zusammengeführte Zellen hat.


**Returns:**
java.lang.Boolean -  true  wenn die Tabelle zusammengeführte Zellen hat; andernfalls  false .  null  wenn sie nicht gesetzt ist.

### getMinRowCount() {#getMinRowCount--}
```
public Integer getMinRowCount()
```


Liefert die minimale Anzahl der Tabellenzeilen.


**Returns:**
java.lang.Integer - Ein ganzzahliger Wert, der die minimale Anzahl der Tabellenzeilen darstellt;  null  wenn er nicht gesetzt ist.

### getMinColumnCount() {#getMinColumnCount--}
```
public Integer getMinColumnCount()
```


Liefert die minimale Anzahl der Tabellenspalten.


**Returns:**
java.lang.Integer - Ein ganzzahliger Wert, der die minimale Anzahl der Tabellenspalten darstellt;  null  wenn er nicht gesetzt ist.

### getMinVerticalSpace() {#getMinVerticalSpace--}
```
public Integer getMinVerticalSpace()
```


Liefert den minimalen Abstand zwischen den Tabellenspalten.


**Returns:**
java.lang.Integer - Ein ganzzahliger Wert, der den minimalen Abstand zwischen den Tabellenspalten darstellt;  null  wenn er nicht gesetzt ist.

### scale(double factor) {#scale-double-}
```
public TemplateTableParameters scale(double factor)
```


Erstellt eine Kopie dieser Parameter, wobei alle Koordinaten um den angegebenen Faktor skaliert werden.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Faktor | double | Der Skalierungsfaktor. |
|

**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - A new [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) with scaled coordinates.


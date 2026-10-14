---
title: "TemplateTableParameters"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller parametrar för tabellidentifieringsalgoritmerna."
type: docs
weight: 22
url: /sv/java/com.groupdocs.parser.templates/templatetableparameters/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableParameters
```

Tillhandahåller parametrar för tabellidentifieringsalgoritmerna.

Det finns två algoritmer för att upptäcka en tabell:

* Allows to detect a table in the rectangular area with set columns. This algorithm is useful for simple tables (without merged columns) and provides more accurate detection.
* Allows to detect a table in any place on the page. This is a more complex algorithm. It can detect tables in any place on the page. Additional parameters help to detect a table more correctly.

I vissa fall när algoritmer inte kan upptäcka en tabell eller gör det på ett inexakt sätt används klassen [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout).

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--) | Initierar en ny instans av klassen [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters). |
|
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-) | Initierar en ny instans av klassen [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Hämtar det rektangulära området som innehåller tabellen. |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | Hämtar kolumnseparatorerna för tabellen. |
|
|  | [hasMergedCells()](#hasMergedCells--) | Hämtar värdet som indikerar om tabellen har sammanslagna celler. |
|
|  | [getMinRowCount()](#getMinRowCount--) | Hämtar det minsta antalet rader i tabellen. |
|
|  | [getMinColumnCount()](#getMinColumnCount--) | Hämtar det minsta antalet kolumner i tabellen. |
|
|  | [getMinVerticalSpace()](#getMinVerticalSpace--) | Hämtar det minsta utrymmet mellan tabellkolumnerna. |
|
|  | [scale(double factor)](#scale-double-) | Skapar en kopia av dessa parametrar med alla koordinater skalade med den angivna faktorn. |
|
### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)
```


Initierar en ny instans av klassen [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området som innehåller tabellen. |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | Tabellens kolumnseparatorer. |
|

### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)
```


Initierar en ny instans av klassen [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området som innehåller tabellen. |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | Tabellens kolumnseparatorer. |
|
|  | mergedCells | java.lang.Boolean | Värdet som indikerar om tabellen har sammanslagna celler. |
|
|  | minRowCount | java.lang.Integer | Det minsta antalet rader i tabellen. |
|
|  | minColumnCount | java.lang.Integer | Det minsta antalet kolumner i tabellen. |
|
|  | minVerticalSpace | java.lang.Integer | Det minsta utrymmet mellan tabellkolumnerna. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Hämtar det rektangulära området som innehåller tabellen.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table;  null  if it isn't set.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


Hämtar kolumnseparatorerna för tabellen.


**Returns:**
java.util.List<java.lang.Double> - En samling av double‑värden som representerar x‑koordinater för tabellkolumnseparatorerna;  null  om den inte är inställd.

### hasMergedCells() {#hasMergedCells--}
```
public Boolean hasMergedCells()
```


Hämtar värdet som indikerar om tabellen har sammanslagna celler.


**Returns:**
java.lang.Boolean -  true  om tabellen har sammanslagna celler; annars,  false .  null  om den inte är inställd.

### getMinRowCount() {#getMinRowCount--}
```
public Integer getMinRowCount()
```


Hämtar det minsta antalet rader i tabellen.


**Returns:**
java.lang.Integer - Ett heltal som representerar det minsta antalet rader i tabellen;  null  om den inte är inställd.

### getMinColumnCount() {#getMinColumnCount--}
```
public Integer getMinColumnCount()
```


Hämtar det minsta antalet kolumner i tabellen.


**Returns:**
java.lang.Integer - Ett heltal som representerar det minsta antalet kolumner i tabellen;  null  om den inte är inställd.

### getMinVerticalSpace() {#getMinVerticalSpace--}
```
public Integer getMinVerticalSpace()
```


Hämtar det minsta utrymmet mellan tabellkolumnerna.


**Returns:**
java.lang.Integer - Ett heltal som representerar det minsta utrymmet mellan tabellkolumnerna;  null  om den inte är inställd.

### scale(double factor) {#scale-double-}
```
public TemplateTableParameters scale(double factor)
```


Skapar en kopia av dessa parametrar med alla koordinater skalade med den angivna faktorn.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | faktor | double | Skalfaktorn. |
|

**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - A new [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) with scaled coordinates.


---
title: "TemplateTableParameters"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt parameters voor de tabeldetectie-algoritmen."
type: docs
weight: 22
url: /nl/java/com.groupdocs.parser.templates/templatetableparameters/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableParameters
```

Biedt parameters voor de tabeldetectie-algoritmen.

Er zijn twee algoritmen om een tabel te detecteren:

* Allows to detect a table in the rectangular area with set columns. This algorithm is useful for simple tables (without merged columns) and provides more accurate detection.
* Allows to detect a table in any place on the page. This is a more complex algorithm. It can detect tables in any place on the page. Additional parameters help to detect a table more correctly.

In sommige gevallen wanneer algoritmen geen tabel kunnen detecteren of dit op een onnauwkeurige manier doen, wordt de klasse [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) gebruikt.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--) | Initialiseert een nieuwe instantie van de klasse [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters). |
|
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-) | Initialiseert een nieuwe instantie van de klasse [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters). |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Haalt het rechthoekige gebied op dat de tabel bevat. |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | Haalt de scheidingstekens van de tabelkolommen op. |
|
|  | [hasMergedCells()](#hasMergedCells--) | Haalt de waarde op die aangeeft of de tabel samengevoegde cellen heeft. |
|
|  | [getMinRowCount()](#getMinRowCount--) | Haalt het minimum aantal rijen van de tabel op. |
|
|  | [getMinColumnCount()](#getMinColumnCount--) | Haalt het minimum aantal kolommen van de tabel op. |
|
|  | [getMinVerticalSpace()](#getMinVerticalSpace--) | Haalt de minimale ruimte tussen de tabelkolommen op. |
|
|  | [scale(double factor)](#scale-double-) | Maakt een kopie van deze parameters waarbij alle coördinaten worden geschaald met de opgegeven factor. |
|
### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)
```


Initialiseert een nieuwe instantie van de klasse [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied dat de tabel bevat. |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | De scheidingstekens van de tabelkolommen. |
|

### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)
```


Initialiseert een nieuwe instantie van de klasse [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied dat de tabel bevat. |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | De scheidingstekens van de tabelkolommen. |
|
|  | mergedCells | java.lang.Boolean | De waarde die aangeeft of de tabel samengevoegde cellen heeft. |
|
|  | minRowCount | java.lang.Integer | Het minimum aantal tabelrijen. |
|
|  | minColumnCount | java.lang.Integer | Het minimum aantal tabelkolommen. |
|
|  | minVerticalSpace | java.lang.Integer | De minimumruimte tussen de tabelkolommen. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Haalt het rechthoekige gebied op dat de tabel bevat.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table;  null  if it isn't set.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


Haalt de scheidingstekens van de tabelkolommen op.


**Returns:**
java.util.List<java.lang.Double> - Een collectie van double-waarden die de x-coördinaten van de scheidingslijnen van de tabelkolommen vertegenwoordigen;  null  als deze niet is ingesteld.

### hasMergedCells() {#hasMergedCells--}
```
public Boolean hasMergedCells()
```


Haalt de waarde op die aangeeft of de tabel samengevoegde cellen heeft.


**Returns:**
java.lang.Boolean -  true  als de tabel samengevoegde cellen heeft; anders,  false .  null  als deze niet is ingesteld.

### getMinRowCount() {#getMinRowCount--}
```
public Integer getMinRowCount()
```


Haalt het minimum aantal rijen van de tabel op.


**Returns:**
java.lang.Integer - Een geheel getal dat het minimum aantal tabelrijen vertegenwoordigt;  null  als deze niet is ingesteld.

### getMinColumnCount() {#getMinColumnCount--}
```
public Integer getMinColumnCount()
```


Haalt het minimum aantal kolommen van de tabel op.


**Returns:**
java.lang.Integer - Een geheel getal dat het minimum aantal tabelkolommen vertegenwoordigt;  null  als deze niet is ingesteld.

### getMinVerticalSpace() {#getMinVerticalSpace--}
```
public Integer getMinVerticalSpace()
```


Haalt de minimale ruimte tussen de tabelkolommen op.


**Returns:**
java.lang.Integer - Een geheel getal dat de minimumruimte tussen de tabelkolommen vertegenwoordigt;  null  als deze niet is ingesteld.

### scale(double factor) {#scale-double-}
```
public TemplateTableParameters scale(double factor)
```


Maakt een kopie van deze parameters waarbij alle coördinaten worden geschaald met de opgegeven factor.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | factor | double | De schaalfactor. |
|

**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - A new [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) with scaled coordinates.


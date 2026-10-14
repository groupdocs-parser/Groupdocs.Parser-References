---
title: "TemplateTableLayout"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller malltabellens layout som används av klassen för att definiera tabellposition."
type: docs
weight: 21
url: /sv/java/com.groupdocs.parser.templates/templatetablelayout/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableLayout
```

Tillhandahåller malltabellens layout som används av klassen [TemplateTable](../../com.groupdocs.parser.templates/templatetable) för att definiera tabellposition.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)](#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--) | Initierar en ny instans av klassen [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Hämtar det rektangulära området som innehåller tabellen. |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | Hämtar kolumnseparatorerna för tabellen. |
|
|  | [getHorizontalSeparators()](#getHorizontalSeparators--) | Hämtar radseparatorerna för tabellen. |
|
|  | [moveTo(Point point)](#moveTo-com.groupdocs.parser.data.Point-) | Skapar en ny layout med samma storlek, separatorer och position i punkten. |
|
|  | [scale(double factor)](#scale-double-) | Skapar en kopia av denna layout med alla koordinater skalade med den angivna faktorn. |
|
### TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators) {#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--}
```
public TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)
```


Initierar en ny instans av klassen [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | Tabellens kolumnseparatorer. |
|
|  | horizontalSeparators | java.lang.Iterable<java.lang.Double> | Tabellens radseparatorer. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Hämtar det rektangulära området som innehåller tabellen.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


Hämtar kolumnseparatorerna för tabellen.


**Returns:**
java.util.List<java.lang.Double> - En samling av dubbelvärden som representerar x-koordinaterna för tabellens kolumnseparatorer.

### getHorizontalSeparators() {#getHorizontalSeparators--}
```
public List<Double> getHorizontalSeparators()
```


Hämtar radseparatorerna för tabellen.


**Returns:**
java.util.List<java.lang.Double> - En samling av dubbelvärden som representerar y-koordinaterna för tabellens radseparatorer.

### moveTo(Point point) {#moveTo-com.groupdocs.parser.data.Point-}
```
public TemplateTableLayout moveTo(Point point)
```


Skapar en ny layout med samma storlek, separatorer och position i punkten.

Denna funktionalitet möjliggör att flytta Table Layout.

Till exempel har ett dokument tabeller på varje sida (eller en uppsättning dokument med en tabell på sidan).
Dessa tabeller skiljer sig åt i position och innehåll, men har samma kolumner och rader. I det här fallet en användare
kan definiera [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) objektet vid (0, 0) en gång och sedan flytta det till den bestämda tabellens plats.

Om tabellens position beror på ett annat objekt på sidan, kan en användare definiera [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) objektet
baserat på malldokumentet och sedan flytta det enligt ett ankareobjekt. Till exempel, om detta är en sammanfattningstabell
och den följs av en detaljtabel (som kan innehålla ett annat antal rader). I det här fallet kan en användare definiera
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object on template document (with the known details table rectangle) and then move
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object according to the difference of details table rectangle of template and real document.


moveTo(Point)
metoden returnerar en kopia av det aktuella objektet. En användare kan skicka vilka koordinater som helst
(även negativa - då kommer layouten att flyttas åt vänster/upp).

````
// Create a table layout
 TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 0.0, 25.0, 150.0, 180.0, 230.0 }),
     java.util.Arrays.asList(new Double[] { 0.0, 15.0, 30.0, 45.0, 60.0, 75.0 }));
 // Print a rectangle
 Rectangle rect = layout.getRectangle();
 // Prints: pos: (0, 0) size: (230, 75)
 System.out.println(String.format("pos: (%d, %d) size: (%d, %d)",
         rect.getLeft(), rect.getTop(),
         rect.getSize().getWidth(), rect.getSize().getHeight()));
 // Move layout to the definite table location
 TemplateTableLayout movedLayout = layout.moveTo(new Point(315, 250));
 // Ensure that the first separators are moved:
 System.out.println(movedLayout.getVerticalSeparators().get(0)); // prints: 315
 System.out.println(movedLayout.getHorizontalSeparators().get(0)); // prints: 250
 Rectangle movedRect = movedLayout.getRectangle();
 // Prints: pos: (315, 250) size: (230, 75)
 System.out.println(String.format("pos: (%d, %d) size: (%d, %d)",
         movedRect.getLeft(), movedRect.getTop(),
         movedRect.getSize().getWidth(), movedRect.getSize().getHeight()));
 // movedLayout object is a copy of layout object, thus we can tune separators without the impact on the original layout:
 movedLayout.getHorizontalSeparators().add(90.0);
 System.out.println(movedLayout.getHorizontalSeparators().size()); // prints: 7
 System.out.println(layout.getHorizontalSeparators().size()); // prints: 6
 
````



**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | point | [Point](../../com.groupdocs.parser.data/point) | Positionen för den nya layouten. |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new layout with the same size, separators and position in the point.

### scale(double factor) {#scale-double-}
```
public TemplateTableLayout scale(double factor)
```


Skapar en kopia av denna layout med alla koordinater skalade med den angivna faktorn.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | faktor | double | Skalfaktorn. |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) with scaled separators.


---
title: "TemplateTableLayout"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt de sjabloontabelindeling die wordt gebruikt door de klasse om de tabelpositie te definiëren."
type: docs
weight: 21
url: /nl/java/com.groupdocs.parser.templates/templatetablelayout/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableLayout
```

Biedt de sjabloontabelindeling die wordt gebruikt door de klasse [TemplateTable](../../com.groupdocs.parser.templates/templatetable) om de tabelpositie te definiëren.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)](#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--) | Initialiseert een nieuw exemplaar van de klasse [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout). |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Haalt het rechthoekige gebied op dat de tabel bevat. |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | Haalt de scheidingstekens van de tabelkolommen op. |
|
|  | [getHorizontalSeparators()](#getHorizontalSeparators--) | Haalt de scheidingstekens van de tabelrijen op. |
|
|  | [moveTo(Point point)](#moveTo-com.groupdocs.parser.data.Point-) | Maakt een nieuwe lay-out met dezelfde grootte, scheidingstekens en positie in het punt. |
|
|  | [scale(double factor)](#scale-double-) | Maakt een kopie van deze lay-out waarbij alle coördinaten worden geschaald met de opgegeven factor. |
|
### TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators) {#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--}
```
public TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)
```


Initialiseert een nieuw exemplaar van de klasse [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | De scheidingstekens van de tabelkolommen. |
|
|  | horizontalSeparators | java.lang.Iterable<java.lang.Double> | De scheidingstekens van de tabelrijen. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Haalt het rechthoekige gebied op dat de tabel bevat.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


Haalt de scheidingstekens van de tabelkolommen op.


**Returns:**
java.util.List<java.lang.Double> - Een collectie van double-waarden die de x-coördinaten van de scheidingstekens van de tabelkolommen vertegenwoordigen.

### getHorizontalSeparators() {#getHorizontalSeparators--}
```
public List<Double> getHorizontalSeparators()
```


Haalt de scheidingstekens van de tabelrijen op.


**Returns:**
java.util.List<java.lang.Double> - Een collectie van double-waarden die de y-coördinaten van de scheidingstekens van de tabelrijen vertegenwoordigen.

### moveTo(Point point) {#moveTo-com.groupdocs.parser.data.Point-}
```
public TemplateTableLayout moveTo(Point point)
```


Maakt een nieuwe lay-out met dezelfde grootte, scheidingstekens en positie in het punt.

Deze functionaliteit maakt het mogelijk om Table Layout te verplaatsen.

Bijvoorbeeld, een document heeft tabellen op elke pagina (of een reeks documenten met een tabel op de pagina).
Deze tabellen verschillen in positie en inhoud, maar hebben dezelfde kolommen en rijen. In dit geval een gebruiker
kan een [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object op (0, 0) definiëren en vervolgens verplaatsen naar de locatie van de definitieve tabel.

Als de tabelpositie afhankelijk is van een ander object op de pagina, kan een gebruiker een [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object definiëren
gebaseerd op het sjabloondocument en vervolgens verplaatsen volgens een ankerobject. Bijvoorbeeld, als dit een samenvattende tabel is
en deze wordt gevolgd door een detailtabel (die een verschillend aantal rijen kan bevatten). In dit geval kan een gebruiker definiëren
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object on template document (with the known details table rectangle) and then move
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object according to the difference of details table rectangle of template and real document.


moveTo(Point)
methode retourneert een kopie van het huidige object. Een gebruiker kan elke coördinaat doorgeven
(zelfs negatief - dan wordt de layout naar links/boven verplaatst).

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | point | [Point](../../com.groupdocs.parser.data/point) | De positie van de nieuwe layout. |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new layout with the same size, separators and position in the point.

### scale(double factor) {#scale-double-}
```
public TemplateTableLayout scale(double factor)
```


Maakt een kopie van deze lay-out waarbij alle coördinaten worden geschaald met de opgegeven factor.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | factor | double | De schaalfactor. |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) with scaled separators.


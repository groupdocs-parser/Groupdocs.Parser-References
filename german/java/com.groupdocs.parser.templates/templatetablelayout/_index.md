---
title: "TemplateTableLayout"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt das Vorlagentabellenlayout bereit, das von der Klasse verwendet wird, um die Tabellenposition zu definieren."
type: docs
weight: 21
url: /de/java/com.groupdocs.parser.templates/templatetablelayout/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableLayout
```

Stellt das Vorlagen-Tabellenlayout bereit, das von der Klasse [TemplateTable](../../com.groupdocs.parser.templates/templatetable) verwendet wird, um die Tabellenposition zu definieren.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)](#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--) | Initialisiert eine neue Instanz der Klasse [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Gibt den rechteckigen Bereich zurück, der die Tabelle enthält. |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | Gibt die Trennlinien der Tabellenspalten zurück. |
|
|  | [getHorizontalSeparators()](#getHorizontalSeparators--) | Gibt die Trennlinien der Tabellenzeilen zurück. |
|
|  | [moveTo(Point point)](#moveTo-com.groupdocs.parser.data.Point-) | Erstellt ein neues Layout mit derselben Größe, denselben Trennlinien und derselben Position im Punkt. |
|
|  | [scale(double factor)](#scale-double-) | Erstellt eine Kopie dieses Layouts, wobei alle Koordinaten um den angegebenen Faktor skaliert werden. |
|
### TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators) {#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--}
```
public TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)
```


Initialisiert eine neue Instanz der Klasse [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | Die Trennlinien der Tabellenspalten. |
|
|  | horizontalSeparators | java.lang.Iterable<java.lang.Double> | Die Trennlinien der Tabellenzeilen. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Gibt den rechteckigen Bereich zurück, der die Tabelle enthält.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


Gibt die Trennlinien der Tabellenspalten zurück.


**Returns:**
java.util.List<java.lang.Double> - Eine Sammlung von Double-Werten, die die x-Koordinaten der Trennlinien der Tabellenspalten darstellen.

### getHorizontalSeparators() {#getHorizontalSeparators--}
```
public List<Double> getHorizontalSeparators()
```


Gibt die Trennlinien der Tabellenzeilen zurück.


**Returns:**
java.util.List<java.lang.Double> - Eine Sammlung von Double-Werten, die die y-Koordinaten der Trennlinien der Tabellenzeilen darstellen.

### moveTo(Point point) {#moveTo-com.groupdocs.parser.data.Point-}
```
public TemplateTableLayout moveTo(Point point)
```


Erstellt ein neues Layout mit derselben Größe, denselben Trennlinien und derselben Position im Punkt.

Diese Funktionalität ermöglicht das Verschieben des Tabellenlayouts.

Zum Beispiel hat ein Dokument auf jeder Seite Tabellen (oder ein Satz von Dokumenten mit einer Tabelle auf der Seite).
Diese Tabellen unterscheiden sich in Position und Inhalt, haben aber dieselben Spalten und Zeilen. In diesem Fall ein Benutzer
kann ein [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout)-Objekt bei (0, 0) einmal definieren und es dann an die Position der konkreten Tabelle verschieben.

Wenn die Tabellenposition von einem anderen Objekt der Seite abhängt, kann ein Benutzer ein [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout)-Objekt definieren
basierend auf dem Vorlagendokument und es dann gemäß einem Ankerobjekt verschieben. Zum Beispiel, wenn dies eine Zusammenfassungstabelle ist
und ihr folgt eine Detailtabelle (die eine unterschiedliche Zeilenanzahl enthalten kann). In diesem Fall kann ein Benutzer definieren
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object on template document (with the known details table rectangle) and then move
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object according to the difference of details table rectangle of template and real document.


moveTo(Point)
Methode gibt eine Kopie des aktuellen Objekts zurück. Ein Benutzer kann beliebige Koordinaten übergeben
(auch negative – dann wird das Layout nach links/oben verschoben).

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | point | [Point](../../com.groupdocs.parser.data/point) | Die Position des neuen Layouts. |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new layout with the same size, separators and position in the point.

### scale(double factor) {#scale-double-}
```
public TemplateTableLayout scale(double factor)
```


Erstellt eine Kopie dieses Layouts, wobei alle Koordinaten um den angegebenen Faktor skaliert werden.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Faktor | double | Der Skalierungsfaktor. |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) with scaled separators.


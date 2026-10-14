---
title: "TemplateFixedPosition"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt eine Vorlagenfeldposition bereit, die durch den rechteckigen Bereich definiert ist."
type: docs
weight: 13
url: /de/java/com.groupdocs.parser.templates/templatefixedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateFixedPosition extends TemplatePosition
```

Stellt eine Vorlagenfeldposition bereit, die durch den rechteckigen Bereich definiert ist.

Dies ist der einfachste Weg, die Feldposition zu definieren. Es erfordert, einen rechteckigen Bereich auf der Seite festzulegen, der
den Feldwert. Der gesamte Text, der (auch teilweise) im rechteckigen Bereich enthalten ist, wird als Wert extrahiert:

````
// Create a fixed template field with "Address" name which is bounded by a rectangle at the position (35, 160) and with the size (110, 20)
 TemplateField templateField = new TemplateField(
     new TemplateFixedPosition(new Rectangle(new Point(35, 160), new Size(110, 20))),
     "Address");
 
````


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [TemplateFixedPosition(Rectangle rectangle)](#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-) | Initialisiert eine neue Instanz der Klasse [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Liefert den rechteckigen Bereich, der das Vorlagenfeld enthält. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateFixedPosition(Rectangle rectangle) {#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-}
```
public TemplateFixedPosition(Rectangle rectangle)
```


Initialisiert eine neue Instanz der Klasse [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Der rechteckige Bereich, der das Vorlagenfeld enthält. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Liefert den rechteckigen Bereich, der das Vorlagenfeld enthält.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template field.

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


Erstellt eine Kopie der aktuellen Position, wobei alle Koordinaten um den angegebenen Faktor skaliert werden.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Faktor | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)

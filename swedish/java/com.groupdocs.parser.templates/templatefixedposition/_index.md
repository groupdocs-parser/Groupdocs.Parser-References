---
title: "TemplateFixedPosition"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller en mallfältposition som definieras av det rektangulära området."
type: docs
weight: 13
url: /sv/java/com.groupdocs.parser.templates/templatefixedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateFixedPosition extends TemplatePosition
```

Tillhandahåller en mallfältposition som definieras av det rektangulära området.

Detta är det enklaste sättet att definiera fältpositionen. Det kräver att man anger ett rektangulärt område på sidan som begränsar
fältvärdet. All text som finns (även delvis) i det rektangulära området kommer att extraheras som ett värde:

````
// Create a fixed template field with "Address" name which is bounded by a rectangle at the position (35, 160) and with the size (110, 20)
 TemplateField templateField = new TemplateField(
     new TemplateFixedPosition(new Rectangle(new Point(35, 160), new Size(110, 20))),
     "Address");
 
````


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [TemplateFixedPosition(Rectangle rectangle)](#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-) | Initierar en ny instans av klassen [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Hämtar det rektangulära området som innehåller mallfältet. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateFixedPosition(Rectangle rectangle) {#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-}
```
public TemplateFixedPosition(Rectangle rectangle)
```


Initierar en ny instans av klassen [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området som innehåller mallfältet. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Hämtar det rektangulära området som innehåller mallfältet.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template field.

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


Skapar en kopia av den aktuella positionen med alla koordinater skalade med den angivna faktorn.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| faktor | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)

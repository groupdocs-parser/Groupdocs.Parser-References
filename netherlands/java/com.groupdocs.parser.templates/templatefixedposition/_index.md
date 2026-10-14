---
title: "TemplateFixedPosition"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt een sjabloon-veldpositie die wordt gedefinieerd door het rechthoekige gebied."
type: docs
weight: 13
url: /nl/java/com.groupdocs.parser.templates/templatefixedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateFixedPosition extends TemplatePosition
```

Biedt een sjabloon-veldpositie die wordt gedefinieerd door het rechthoekige gebied.

Dit is de eenvoudigste manier om de veldpositie te definiëren. Het vereist het instellen van een rechthoekig gebied op de pagina dat begrenst
de veldwaarde. Alle tekst die (zelfs gedeeltelijk) in het rechthoekige gebied zit, wordt geëxtraheerd als een waarde:

````
// Create a fixed template field with "Address" name which is bounded by a rectangle at the position (35, 160) and with the size (110, 20)
 TemplateField templateField = new TemplateField(
     new TemplateFixedPosition(new Rectangle(new Point(35, 160), new Size(110, 20))),
     "Address");
 
````


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [TemplateFixedPosition(Rectangle rectangle)](#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-) | Initialiseert een nieuw exemplaar van de [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Haalt het rechthoekige gebied op dat het sjabloonveld bevat. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateFixedPosition(Rectangle rectangle) {#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-}
```
public TemplateFixedPosition(Rectangle rectangle)
```


Initialiseert een nieuw exemplaar van de [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied dat het sjabloonveld bevat. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Haalt het rechthoekige gebied op dat het sjabloonveld bevat.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template field.

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


Maakt een kopie van de huidige positie waarbij alle coördinaten worden geschaald met de opgegeven factor.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| factor | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)

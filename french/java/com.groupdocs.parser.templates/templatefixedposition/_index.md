---
title: "TemplateFixedPosition"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit une position de champ de modèle définie par la zone rectangulaire."
type: docs
weight: 13
url: /fr/java/com.groupdocs.parser.templates/templatefixedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateFixedPosition extends TemplatePosition
```

Fournit une position de champ de modèle définie par la zone rectangulaire.

C'est la façon la plus simple de définir la position du champ. Elle nécessite de définir une zone rectangulaire sur la page qui encadre
la valeur du champ. Tout le texte qui se trouve (même partiellement) dans la zone rectangulaire sera extrait comme valeur :

````
// Create a fixed template field with "Address" name which is bounded by a rectangle at the position (35, 160) and with the size (110, 20)
 TemplateField templateField = new TemplateField(
     new TemplateFixedPosition(new Rectangle(new Point(35, 160), new Size(110, 20))),
     "Address");
 
````


## Constructors

| Constructor | Description |
| --- | --- |
|  | [TemplateFixedPosition(Rectangle rectangle)](#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-) | Initialise une nouvelle instance de la classe [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Obtient la zone rectangulaire qui contient le champ du modèle. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateFixedPosition(Rectangle rectangle) {#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-}
```
public TemplateFixedPosition(Rectangle rectangle)
```


Initialise une nouvelle instance de la classe [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | La zone rectangulaire qui contient le champ du modèle. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Obtient la zone rectangulaire qui contient le champ du modèle.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template field.

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


Crée une copie de la position actuelle avec toutes les coordonnées mises à l'échelle par le facteur donné.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| factor | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)

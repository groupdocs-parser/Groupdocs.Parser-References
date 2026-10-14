---
title: "TemplateTableLayout"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit la mise en page du tableau modèle qui est utilisée par la classe pour définir la position du tableau."
type: docs
weight: 21
url: /fr/java/com.groupdocs.parser.templates/templatetablelayout/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableLayout
```

Fournit la mise en page du tableau modèle qui est utilisée par la classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable) pour définir la position du tableau.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)](#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--) | Initialise une nouvelle instance de la classe [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Obtient la zone rectangulaire qui contient le tableau. |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | Obtient les séparateurs de colonnes du tableau. |
|
|  | [getHorizontalSeparators()](#getHorizontalSeparators--) | Obtient les séparateurs de lignes du tableau. |
|
|  | [moveTo(Point point)](#moveTo-com.groupdocs.parser.data.Point-) | Crée une nouvelle mise en page avec la même taille, les mêmes séparateurs et la même position dans le point. |
|
|  | [scale(double factor)](#scale-double-) | Crée une copie de cette mise en page avec toutes les coordonnées mises à l'échelle par le facteur donné. |
|
### TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators) {#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--}
```
public TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)
```


Initialise une nouvelle instance de la classe [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | Les séparateurs de colonnes du tableau. |
|
|  | horizontalSeparators | java.lang.Iterable<java.lang.Double> | Les séparateurs de lignes du tableau. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Obtient la zone rectangulaire qui contient le tableau.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


Obtient les séparateurs de colonnes du tableau.


**Returns:**
java.util.List<java.lang.Double> - Une collection de valeurs double qui représentent les coordonnées x des séparateurs de colonnes du tableau.

### getHorizontalSeparators() {#getHorizontalSeparators--}
```
public List<Double> getHorizontalSeparators()
```


Obtient les séparateurs de lignes du tableau.


**Returns:**
java.util.List<java.lang.Double> - Une collection de valeurs double qui représentent les coordonnées y des séparateurs de lignes du tableau.

### moveTo(Point point) {#moveTo-com.groupdocs.parser.data.Point-}
```
public TemplateTableLayout moveTo(Point point)
```


Crée une nouvelle mise en page avec la même taille, les mêmes séparateurs et la même position dans le point.

Cette fonctionnalité permet de déplacer le Table Layout.

Par exemple, un document possède des tables sur chaque page (ou un ensemble de documents avec une table sur la page).
Ces tables diffèrent par leur position et leur contenu, mais ont les mêmes colonnes et lignes. Dans ce cas, un utilisateur
peut définir l'objet [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) à (0, 0) une fois, puis le déplacer vers l'emplacement de la table définie.

Si la position de la table dépend d'un autre objet de la page, un utilisateur peut définir l'objet [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) 
basé sur le document modèle et le déplacer ensuite selon un objet d'ancrage. Par exemple, si c'est une table de synthèse
et qu'elle est suivie d'une table de détails (qui peut contenir un nombre différent de lignes). Dans ce cas, un utilisateur peut définir
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object on template document (with the known details table rectangle) and then move
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object according to the difference of details table rectangle of template and real document.


moveTo(Point)
la méthode renvoie une copie de l'objet actuel. Un utilisateur peut fournir n'importe quelles coordonnées
(même négatives - alors la disposition sera déplacée vers la gauche/haut).

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
| Parameter | Type | Description |
| --- | --- | --- |
|  | point | [Point](../../com.groupdocs.parser.data/point) | La position de la nouvelle disposition. |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new layout with the same size, separators and position in the point.

### scale(double factor) {#scale-double-}
```
public TemplateTableLayout scale(double factor)
```


Crée une copie de cette mise en page avec toutes les coordonnées mises à l'échelle par le facteur donné.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | factor | double | Le facteur d'échelle. |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) with scaled separators.


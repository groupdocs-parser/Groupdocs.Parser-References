---
title: "PageAreaOptions"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit les options utilisées pour l'extraction des zones de page."
type: docs
weight: 28
url: /fr/java/com.groupdocs.parser.options/pageareaoptions/
---
**Inheritance:**
java.lang.Object
```
public class PageAreaOptions
```

Fournit les options utilisées pour l'extraction des zones de page.

Une instance de la classe [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) est utilisée comme paramètre dans [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-).
et les méthodes [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-). Voir les exemples d'utilisation là-bas.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [PageAreaOptions(Rectangle rectangle)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-) | Initialise une nouvelle instance de la classe [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) avec la taille de la bordure ignorée. |
|
|  | [PageAreaOptions(Rectangle rectangle, double rectangleTolerance)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-) | Initialise une nouvelle instance de la classe [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Obtient la zone rectangulaire qui contient les zones de page. |
|
|  | [getRectangleTolerance()](#getRectangleTolerance--) | Obtient la taille de la bordure qui est ignorée lorsqu'elle est capturée par la zone rectangulaire. |
|
### PageAreaOptions(Rectangle rectangle) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageAreaOptions(Rectangle rectangle)
```


Initialise une nouvelle instance de la classe [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) avec la taille de la bordure ignorée.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | La zone rectangulaire qui contient les zones de page. |
|

### PageAreaOptions(Rectangle rectangle, double rectangleTolerance) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-}
```
public PageAreaOptions(Rectangle rectangle, double rectangleTolerance)
```


Initialise une nouvelle instance de la classe [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | La zone rectangulaire qui contient les zones de page. |
|
|  | rectangleTolerance | double | La taille de la bordure qui est ignorée lorsqu'elle est capturée par la zone rectangulaire. Elle est mesurée par la fraction de la hauteur d'un élément de texte. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Obtient la zone rectangulaire qui contient les zones de page.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


Obtient la taille de la bordure qui est ignorée lorsqu'elle est capturée par la zone rectangulaire. Elle est mesurée par la fraction de la hauteur d'un élément de texte.


**Returns:**
double - La valeur double de 0 (pas de bordure) à 1 (ignorer tout l'élément).


---
title: "PageArea"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente une classe de base abstraite pour les zones de page utilisées pour représenter des blocs sur la page du document dans la fonctionnalité d'analyse par modèle."
type: docs
weight: 17
url: /fr/java/com.groupdocs.parser.data/pagearea/
---
**Inheritance:**
java.lang.Object
```
public abstract class PageArea
```

Représente une classe de base abstraite pour les zones de page utilisées pour représenter des blocs sur la page du document dans la fonctionnalité d'analyse par modèle.

## Methods

| Method | Description |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Obtient la zone rectangulaire. |
|
|  | [getPage()](#getPage--) | Obtient les informations de la page du document telles que l'index de page et la taille de page. |
|
### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Obtient la zone rectangulaire.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area of the page that contains the page area.

### getPage() {#getPage--}
```
public Page getPage()
```


Obtient les informations de la page du document telles que l'index de page et la taille de page.


**Returns:**
[Page](../../com.groupdocs.parser.data/page) - An instance of [Page](../../com.groupdocs.parser.data/page) class that represents the page that contains the page area.


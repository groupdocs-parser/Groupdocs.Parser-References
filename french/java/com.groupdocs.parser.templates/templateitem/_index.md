---
title: "TemplateItem"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit une classe abstraite de base pour les éléments du modèle."
type: docs
weight: 14
url: /fr/java/com.groupdocs.parser.templates/templateitem/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplateItem
```

Fournit une classe abstraite de base pour les éléments du modèle.

Les classes dérivées de [TemplateItem](../../com.groupdocs.parser.templates/templateitem) sont utilisées dans la collection [Template](../../com.groupdocs.parser.templates/template).

## Methods

| Method | Description |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | Crée une copie de l'élément actuel avec toutes les coordonnées mises à l'échelle par le facteur donné. |
|
|  | [getName()](#getName--) | Obtient le nom de l'élément de modèle. |
|
|  | [getPageIndex()](#getPageIndex--) | Obtient l'index de page de l'élément de modèle. |
|
|  | [getPageWidth()](#getPageWidth--) | Obtient la largeur de la page qui a été utilisée pour créer l'élément de modèle. |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | Obtient une valeur qui indique si un  Name  a été converti en MAJUSCULES. |
|
### scale(double factor) {#scale-double-}
```
public abstract TemplateItem scale(double factor)
```


Crée une copie de l'élément actuel avec toutes les coordonnées mises à l'échelle par le facteur donné.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | factor | double | Le facteur d'échelle. |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - A new [TemplateItem](../../com.groupdocs.parser.templates/templateitem) with scaled coordinates.

### getName() {#getName--}
```
public String getName()
```


Obtient le nom de l'élément de modèle.


**Returns:**
java.lang.String - Une chaîne de caractères en majuscules qui représente le nom de l'élément de modèle.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Obtient l'index de page de l'élément de modèle.


**Returns:**
java.lang.Integer - Une valeur entière qui représente l'index de la page où l'élément de modèle est situé ;  null  si l'élément de modèle est situé sur n'importe quelle page.

### getPageWidth() {#getPageWidth--}
```
public Double getPageWidth()
```


Obtient la largeur de la page qui a été utilisée pour créer l'élément de modèle.


**Returns:**
java.lang.Double - La largeur de la page en pixels ;  null  si la largeur de la page est inconnue.

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


Obtient une valeur qui indique si un  Name  a été converti en MAJUSCULES.


**Returns:**
boolean - Une valeur booléenne qui indique si un  Name  a été converti en MAJUSCULE.


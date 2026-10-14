---
title: "Page"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente les informations de la page du document telles que l'indice de page et la taille de la page."
type: docs
weight: 16
url: /fr/java/com.groupdocs.parser.data/page/
---
**Inheritance:**
java.lang.Object
```
public class Page
```

Représente les informations de la page du document telles que l'index de page et la taille de page. Il est utilisé pour représenter la page qui contient les héritiers de la classe [PageArea](../../com.groupdocs.parser.data/pagearea) dans la fonctionnalité d'analyse par modèle.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [Page(int index, Size size)](#Page-int-com.groupdocs.parser.data.Size-) | Initialise une nouvelle instance de la classe [Page](../../com.groupdocs.parser.data/page). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getIndex()](#getIndex--) | Obtient l'indice de page. |
|
|  | [getSize()](#getSize--) | Obtient la taille de la page. |
|
### Page(int index, Size size) {#Page-int-com.groupdocs.parser.data.Size-}
```
public Page(int index, Size size)
```


Initialise une nouvelle instance de la classe [Page](../../com.groupdocs.parser.data/page).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | indice | int | L'index de la page. |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | La taille de la page. |
|

### getIndex() {#getIndex--}
```
public int getIndex()
```


Obtient l'indice de page.


**Returns:**
int - Un index de page basé sur zéro.

### getSize() {#getSize--}
```
public Size getSize()
```


Obtient la taille de la page.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the page.


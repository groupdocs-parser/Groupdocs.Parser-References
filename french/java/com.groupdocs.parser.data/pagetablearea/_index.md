---
title: "PageTableArea"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente une zone de tableau de page utilisée pour représenter un tableau dans la fonctionnalité d'analyse par modèle."
type: docs
weight: 22
url: /fr/java/com.groupdocs.parser.data/pagetablearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTableArea extends PageArea
```

Représente une zone de tableau de page utilisée pour représenter un tableau dans la fonctionnalité d'analyse par modèle.

[PageTableArea](../../com.groupdocs.parser.data/pagetablearea) class is used to organize inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class in table structure.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)](#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initialise une nouvelle instance de la classe [PageTableArea](../../com.groupdocs.parser.data/pagetablearea). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getCells()](#getCells--) | Obtient la collection de cellules. |
|
|  | [getRowCount()](#getRowCount--) | Obtient le nombre total de lignes du tableau. |
|
|  | [getColumnCount()](#getColumnCount--) | Obtient le nombre total de colonnes du tableau. |
|
|  | [getRowHeight(int rowIndex)](#getRowHeight-int-) | Renvoie la hauteur de la ligne. |
|
|  | [getColumnWidth(int columnIndex)](#getColumnWidth-int-) | Renvoie la largeur de la colonne. |
|
|  | [getCell(int rowIndex, int columnIndex)](#getCell-int-int-) | Obtient la cellule du tableau par les index de ligne et de colonne. |
|
### PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle) {#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)
```


Initialise une nouvelle instance de la classe [PageTableArea](../../com.groupdocs.parser.data/pagetablearea).

Remarque : le projet C# marque ce constructeur comme
interne
(commit 954951f). En Java, "internal-to-the-assembly"
ne se traduit pas proprement en package-private car les producteurs (
WordProcessingParser
,
TableAreaParser
,
etc.) résident dans
com.groupdocs.parser
, pas
com.groupdocs.parser.data
. Le constructeur est donc conservé

public
ainsi la construction inter-packages fonctionne toujours.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | lignes | java.lang.Iterable<java.lang.Double> | La collection des hauteurs de lignes. |
|
|  | colonnes | java.lang.Iterable<java.lang.Double> | La collection des largeurs de colonnes. |
|
|  | cellules | java.lang.Iterable<com.groupdocs.parser.data.PageTableAreaCell> | La collection des cellules. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | La page qui contient le tableau. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | La zone rectangulaire qui contient le tableau. |
|

### getCells() {#getCells--}
```
public Collection<PageTableAreaCell> getCells()
```


Obtient la collection de cellules. Une collection en lecture seule simple de cellules de tableau.


**Returns:**
java.util.Collection<com.groupdocs.parser.data.PageTableAreaCell> - Une collection de cellules de tableau

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Obtient le nombre total de lignes du tableau.


**Returns:**
int - Une valeur entière qui contient le nombre total de lignes du tableau.

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Obtient le nombre total de colonnes du tableau.


**Returns:**
int - Une valeur entière qui contient le nombre total de colonnes du tableau.

### getRowHeight(int rowIndex) {#getRowHeight-int-}
```
public double getRowHeight(int rowIndex)
```


Renvoie la hauteur de la ligne.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | rowIndex | int | L'index basé sur zéro de la ligne. |
|

**Returns:**
double - Une valeur double qui représente la hauteur de la ligne.

### getColumnWidth(int columnIndex) {#getColumnWidth-int-}
```
public double getColumnWidth(int columnIndex)
```


Renvoie la largeur de la colonne.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | columnIndex | int | L'index basé sur zéro de la colonne. |
|

**Returns:**
double - Une valeur double qui représente la largeur de la colonne.

### getCell(int rowIndex, int columnIndex) {#getCell-int-int-}
```
public PageTableAreaCell getCell(int rowIndex, int columnIndex)
```


Obtient la cellule du tableau par les index de ligne et de colonne.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | rowIndex | int | L'index basé sur zéro de la ligne de cellule. |
|
|  | columnIndex | int | L'index basé sur zéro de la colonne de cellule. |
|

**Returns:**
[PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) - An instance of [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) class;  null  if no cell is found.


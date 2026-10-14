---
title: "PageTableAreaCell"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente une cellule de tableau qui est utilisée dans la classe."
type: docs
weight: 23
url: /fr/java/com.groupdocs.parser.data/pagetableareacell/
---
**Inheritance:**
java.lang.Object
```
public class PageTableAreaCell
```

Représente une cellule de tableau qui est utilisée dans la classe [PageTableArea](../../com.groupdocs.parser.data/pagetablearea).

## Constructors

| Constructor | Description |
| --- | --- |
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-) | Initialise une nouvelle instance de la classe [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell). |
|
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-) | Initialise une nouvelle instance de la classe [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getRowIndex()](#getRowIndex--) | Obtient l'index de la ligne. |
|
|  | [getColumnIndex()](#getColumnIndex--) | Obtient l'index de la colonne. |
|
|  | [getRowSpan()](#getRowSpan--) | Obtient le nombre total de lignes contenant la cellule de tableau. |
|
|  | [getColumnSpan()](#getColumnSpan--) | Obtient le nombre total de colonnes contenant la cellule de tableau. |
|
|  | [getPageArea()](#getPageArea--) | Obtient la valeur de la cellule de tableau. |
|
|  | [getText()](#getText--) | Obtient la valeur texte de la cellule de tableau. |
|
### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)
```


Initialise une nouvelle instance de la classe [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | rowIndex | int | L'index basé sur zéro de la ligne. |
|
|  | columnIndex | int | L'index basé sur zéro de la colonne. |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | La valeur de la cellule de tableau. |
|

### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)
```


Initialise une nouvelle instance de la classe [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | rowIndex | int | L'index basé sur zéro de la ligne. |
|
|  | columnIndex | int | L'index basé sur zéro de la colonne. |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | La valeur de la cellule de tableau. |
|
|  | rowSpan | int | Le nombre total de lignes contenant la cellule de tableau. |
|
|  | columnSpan | int | Le nombre total de colonnes contenant la cellule du tableau. |
|

### getRowIndex() {#getRowIndex--}
```
public int getRowIndex()
```


Obtient l'index de la ligne.


**Returns:**
int - Un indice basé sur zéro de la première ligne contenant la cellule du tableau.

### getColumnIndex() {#getColumnIndex--}
```
public int getColumnIndex()
```


Obtient l'index de la colonne.


**Returns:**
int - Un indice basé sur zéro de la première colonne contenant la cellule du tableau.

### getRowSpan() {#getRowSpan--}
```
public int getRowSpan()
```


Obtient le nombre total de lignes contenant la cellule de tableau.


**Returns:**
int - Une valeur entière positive qui représente le nombre total de lignes contenant la cellule du tableau.

### getColumnSpan() {#getColumnSpan--}
```
public int getColumnSpan()
```


Obtient le nombre total de colonnes contenant la cellule de tableau.


**Returns:**
int - Une valeur entière positive qui représente le nombre total de colonnes contenant la cellule du tableau.

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


Obtient la valeur de la cellule de tableau.


**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - Depending on cell [PageArea](../../com.groupdocs.parser.data/pagearea) property can contain any of the inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class.

### getText() {#getText--}
```
public String getText()
```


Obtient la valeur texte de la cellule de tableau.


**Returns:**
java.lang.String - Une chaîne qui représente la valeur texte de la cellule ;  null  si la cellule ne contient pas de valeur texte.


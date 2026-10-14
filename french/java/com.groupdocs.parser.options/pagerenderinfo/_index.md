---
title: "PageRenderInfo"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente les informations sur la façon dont une page est rendue."
type: docs
weight: 30
url: /fr/java/com.groupdocs.parser.options/pagerenderinfo/
---
**Inheritance:**
java.lang.Object
```
public class PageRenderInfo
```

Représente les informations sur la façon dont une page est rendue.

Certains documents (feuilles de calcul, par exemple) ne peuvent pas rendre une page
en une seule image. Pour ces documents, une page est rendue sous forme d'ensemble de tuiles.
Ces tuiles sont placées dans le tableau rectangulaire.


RowCount
et
ColumnCount
représente le nombre total de lignes et de colonnes
de ce tableau. Si la page du document est rendue en une seule image, ces propriétés sont égales à 1.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [PageRenderInfo(int pageNumber, int rowCount, int columnCount)](#PageRenderInfo-int-int-int-) | Initialise une nouvelle instance de la classe [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | Obtient le numéro de page. |
|
|  | [getRowCount()](#getRowCount--) | Obtient le nombre total de lignes de tuiles. |
|
|  | [getColumnCount()](#getColumnCount--) | Obtient le nombre total de colonnes de tuiles. |
|
|  | [getColumn(int tileIndex)](#getColumn-int-) | Renvoie l'index de la colonne où la tuile avec  tileIndex  est placée. |
|
|  | [getRow(int tileIndex)](#getRow-int-) | Renvoie l'index de la ligne où la tuile avec  tileIndex  est placée. |
|
### PageRenderInfo(int pageNumber, int rowCount, int columnCount) {#PageRenderInfo-int-int-int-}
```
public PageRenderInfo(int pageNumber, int rowCount, int columnCount)
```


Initialise une nouvelle instance de la classe [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | pageNumber | int | Le numéro de la page (commence à 1). |
|
|  | rowCount | int | Le nombre total de lignes de tuiles. |
|
|  | columnCount | int | Le nombre total de colonnes de tuiles. |
|

### getPageNumber() {#getPageNumber--}
```
public int getPageNumber()
```


Obtient le numéro de page.


**Returns:**
int - La valeur entière qui représente le numéro de page (commence à 1).

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Obtient le nombre total de lignes de tuiles.


**Returns:**
int - La valeur entière qui représente le nombre total de lignes de tuiles.

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Obtient le nombre total de colonnes de tuiles.


**Returns:**
int - La valeur entière qui représente le nombre total de colonnes de tuiles.

### getColumn(int tileIndex) {#getColumn-int-}
```
public int getColumn(int tileIndex)
```


Renvoie l'index de la colonne où la tuile avec  tileIndex  est placée.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | tileIndex | int | L'index basé sur zéro de la tuile. |
|

**Returns:**
int - La valeur entière basée sur zéro qui représente l'index de la colonne.

### getRow(int tileIndex) {#getRow-int-}
```
public int getRow(int tileIndex)
```


Renvoie l'index de la ligne où la tuile avec  tileIndex  est placée.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | tileIndex | int | L'index basé sur zéro de la tuile. |
|

**Returns:**
int - La valeur entière basée sur zéro qui représente l'index de la ligne.


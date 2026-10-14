---
title: "PageRenderInfo"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt de informatie over hoe een pagina wordt gerenderd voor."
type: docs
weight: 30
url: /nl/java/com.groupdocs.parser.options/pagerenderinfo/
---
**Inheritance:**
java.lang.Object
```
public class PageRenderInfo
```

Stelt de informatie over hoe een pagina wordt gerenderd voor.

Sommige documenten (bijvoorbeeld spreadsheets) kunnen geen pagina renderen
als één afbeelding. Voor die documenten wordt een pagina gerenderd als een reeks tegels.
Deze tegels worden geplaatst in de rechthoekige tabel.


RowCount
en
ColumnCount
vertegenwoordigen het totale aantal rijen en kolommen
van deze tabel. Als een documentpagina wordt gerenderd naar één afbeelding, zijn deze eigenschappen gelijk aan 1.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [PageRenderInfo(int pageNumber, int rowCount, int columnCount)](#PageRenderInfo-int-int-int-) | Initialiseert een nieuw exemplaar van de [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | Haalt het paginanummer op. |
|
|  | [getRowCount()](#getRowCount--) | Haalt het totale aantal tegelrijen op. |
|
|  | [getColumnCount()](#getColumnCount--) | Haalt het totale aantal tegelkolommen op. |
|
|  | [getColumn(int tileIndex)](#getColumn-int-) | Retourneert de index van de kolom waar de tegel met  tileIndex  is geplaatst. |
|
|  | [getRow(int tileIndex)](#getRow-int-) | Retourneert de index van de rij waar de tegel met  tileIndex  is geplaatst. |
|
### PageRenderInfo(int pageNumber, int rowCount, int columnCount) {#PageRenderInfo-int-int-int-}
```
public PageRenderInfo(int pageNumber, int rowCount, int columnCount)
```


Initialiseert een nieuw exemplaar van de [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pageNumber | int | Het nummer van de pagina (begint bij 1). |
|
|  | rowCount | int | Het totale aantal tegelrijen. |
|
|  | columnCount | int | Het totale aantal tegelkolommen. |
|

### getPageNumber() {#getPageNumber--}
```
public int getPageNumber()
```


Haalt het paginanummer op.


**Returns:**
int - De gehele getalwaarde die het paginanummer vertegenwoordigt (begint bij 1).

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Haalt het totale aantal tegelrijen op.


**Returns:**
int - De gehele getalwaarde die het totale aantal tegelrijen vertegenwoordigt.

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Haalt het totale aantal tegelkolommen op.


**Returns:**
int - De gehele getalwaarde die het totale aantal tegelkolommen vertegenwoordigt.

### getColumn(int tileIndex) {#getColumn-int-}
```
public int getColumn(int tileIndex)
```


Retourneert de index van de kolom waar de tegel met  tileIndex  is geplaatst.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | tileIndex | int | De nulgebaseerde index van de tegel. |
|

**Returns:**
int - De nulgebaseerde gehele getalwaarde die de kolomindex vertegenwoordigt.

### getRow(int tileIndex) {#getRow-int-}
```
public int getRow(int tileIndex)
```


Retourneert de index van de rij waar de tegel met  tileIndex  is geplaatst.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | tileIndex | int | De nulgebaseerde index van de tegel. |
|

**Returns:**
int - De nulgebaseerde gehele getalwaarde die de rijindex vertegenwoordigt.


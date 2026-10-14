---
title: "PageRenderInfo"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar information om hur en sida renderas."
type: docs
weight: 30
url: /sv/java/com.groupdocs.parser.options/pagerenderinfo/
---
**Inheritance:**
java.lang.Object
```
public class PageRenderInfo
```

Representerar information om hur en sida renderas.

Vissa dokument (kalkylblad, till exempel) går inte att rendera en sida
som en enda bild. För dessa dokument renderas en sida som en uppsättning av tiles.
Dessa tiles placeras i den rektangulära tabellen.


RowCount
och
ColumnCount
representerar det totala antalet rader och kolumner
för denna tabell. Om dokumentsidan renderas till en enda bild är dessa egenskaper lika med 1.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [PageRenderInfo(int pageNumber, int rowCount, int columnCount)](#PageRenderInfo-int-int-int-) | Initierar en ny instans av klassen [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | Hämtar sidnumret. |
|
|  | [getRowCount()](#getRowCount--) | Hämta det totala antalet tiles-rader. |
|
|  | [getColumnCount()](#getColumnCount--) | Hämta det totala antalet tiles-kolumner. |
|
|  | [getColumn(int tileIndex)](#getColumn-int-) | Returnerar index för kolumn där tile med  tileIndex  är placerad. |
|
|  | [getRow(int tileIndex)](#getRow-int-) | Returnerar index för rad där tile med  tileIndex  är placerad. |
|
### PageRenderInfo(int pageNumber, int rowCount, int columnCount) {#PageRenderInfo-int-int-int-}
```
public PageRenderInfo(int pageNumber, int rowCount, int columnCount)
```


Initierar en ny instans av klassen [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pageNumber | int | Numret på sidan (börjar med 1). |
|
|  | rowCount | int | Det totala antalet kakelrader. |
|
|  | columnCount | int | Det totala antalet kakelkolumner. |
|

### getPageNumber() {#getPageNumber--}
```
public int getPageNumber()
```


Hämtar sidnumret.


**Returns:**
int - Det heltal som representerar sidnumret (börjar med 1).

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Hämta det totala antalet tiles-rader.


**Returns:**
int - Det heltal som representerar det totala antalet kakelrader.

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Hämta det totala antalet tiles-kolumner.


**Returns:**
int - Det heltal som representerar det totala antalet kakelkolumner.

### getColumn(int tileIndex) {#getColumn-int-}
```
public int getColumn(int tileIndex)
```


Returnerar index för kolumn där tile med  tileIndex  är placerad.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | tileIndex | int | Det nollbaserade indexet för kaklet. |
|

**Returns:**
int - Det nollbaserade heltalet som representerar kolumnindexet.

### getRow(int tileIndex) {#getRow-int-}
```
public int getRow(int tileIndex)
```


Returnerar index för rad där tile med  tileIndex  är placerad.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | tileIndex | int | Det nollbaserade indexet för kaklet. |
|

**Returns:**
int - Det nollbaserade heltalet som representerar radindexet.


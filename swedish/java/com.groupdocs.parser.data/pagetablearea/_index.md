---
title: "PageTableArea"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar ett sidområde för tabell som används för att representera en tabell i funktionaliteten för parsning med mall."
type: docs
weight: 22
url: /sv/java/com.groupdocs.parser.data/pagetablearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTableArea extends PageArea
```

Representerar ett sidområde för tabell som används för att representera en tabell i funktionaliteten för parsning med mall.

[PageTableArea](../../com.groupdocs.parser.data/pagetablearea) class is used to organize inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class in table structure.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)](#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initierar en ny instans av klassen [PageTableArea](../../com.groupdocs.parser.data/pagetablearea). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getCells()](#getCells--) | Hämtar samlingen av celler. |
|
|  | [getRowCount()](#getRowCount--) | Hämtar det totala antalet rader i tabellen. |
|
|  | [getColumnCount()](#getColumnCount--) | Hämtar det totala antalet kolumner i tabellen. |
|
|  | [getRowHeight(int rowIndex)](#getRowHeight-int-) | Returnerar radhöjden. |
|
|  | [getColumnWidth(int columnIndex)](#getColumnWidth-int-) | Returnerar kolumnbredden. |
|
|  | [getCell(int rowIndex, int columnIndex)](#getCell-int-int-) | Hämtar tabellcellen efter rad- och kolumnindex. |
|
### PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle) {#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)
```


Initierar en ny instans av klassen [PageTableArea](../../com.groupdocs.parser.data/pagetablearea).

Obs: C#-projektet markerar den här konstruktorn som
intern
(commit 954951f). I Java, "internal-to-the-assembly"
översätts inte smidigt till paketprivat eftersom producenterna (
WordProcessingParser
,
TableAreaParser
,
etc.) finns i
com.groupdocs.parser
, inte
com.groupdocs.parser.data
. Konstruktorn behålls därför

public
så att konstruktion över paket fortfarande fungerar.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rader | java.lang.Iterable<java.lang.Double> | Samlingen av radhöjder. |
|
|  | kolumner | java.lang.Iterable<java.lang.Double> | Samlingen av kolumnbredder. |
|
|  | celler | java.lang.Iterable<com.groupdocs.parser.data.PageTableAreaCell> | Samlingen av celler. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Sidan som innehåller tabellen. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området som innehåller tabellen. |
|

### getCells() {#getCells--}
```
public Collection<PageTableAreaCell> getCells()
```


Hämtar samlingen av celler. En enkel skrivskyddad samling av tabellceller.


**Returns:**
java.util.Collection<com.groupdocs.parser.data.PageTableAreaCell> - En samling av tabellceller

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Hämtar det totala antalet rader i tabellen.


**Returns:**
int - Ett heltalsvärde som innehåller det totala antalet rader i tabellen.

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Hämtar det totala antalet kolumner i tabellen.


**Returns:**
int - Ett heltalsvärde som innehåller det totala antalet kolumner i tabellen.

### getRowHeight(int rowIndex) {#getRowHeight-int-}
```
public double getRowHeight(int rowIndex)
```


Returnerar radhöjden.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rowIndex | int | Det nollbaserade indexet för raden. |
|

**Returns:**
double - Ett dubbelvärde som representerar radens höjd.

### getColumnWidth(int columnIndex) {#getColumnWidth-int-}
```
public double getColumnWidth(int columnIndex)
```


Returnerar kolumnbredden.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | columnIndex | int | Det nollbaserade indexet för kolumnen. |
|

**Returns:**
double - Ett dubbelvärde som representerar kolumnens bredd.

### getCell(int rowIndex, int columnIndex) {#getCell-int-int-}
```
public PageTableAreaCell getCell(int rowIndex, int columnIndex)
```


Hämtar tabellcellen efter rad- och kolumnindex.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rowIndex | int | Det nollbaserade indexet för cellraden. |
|
|  | columnIndex | int | Det nollbaserade indexet för cellkolumnen. |
|

**Returns:**
[PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) - An instance of [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) class;  null  if no cell is found.


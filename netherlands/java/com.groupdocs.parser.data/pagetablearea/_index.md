---
title: "PageTableArea"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt een tabelpaginagebied voor dat wordt gebruikt om een tabel te representeren in de functionaliteit voor parsing op basis van sjablonen."
type: docs
weight: 22
url: /nl/java/com.groupdocs.parser.data/pagetablearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTableArea extends PageArea
```

Stelt een tabelpaginagebied voor dat wordt gebruikt om een tabel te representeren in de functionaliteit voor parsing op basis van sjablonen.

[PageTableArea](../../com.groupdocs.parser.data/pagetablearea) class is used to organize inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class in table structure.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)](#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initialiseert een nieuw exemplaar van de [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getCells()](#getCells--) | Haalt de verzameling cellen op. |
|
|  | [getRowCount()](#getRowCount--) | Haalt het totale aantal rijen van de tabel op. |
|
|  | [getColumnCount()](#getColumnCount--) | Haalt het totale aantal kolommen van de tabel op. |
|
|  | [getRowHeight(int rowIndex)](#getRowHeight-int-) | Retourneert de rijhoogte. |
|
|  | [getColumnWidth(int columnIndex)](#getColumnWidth-int-) | Retourneert de kolombreedte. |
|
|  | [getCell(int rowIndex, int columnIndex)](#getCell-int-int-) | Haalt de tabelcel op op basis van rij- en kolomindexen. |
|
### PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle) {#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)
```


Initialiseert een nieuw exemplaar van de [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) klasse.

Opmerking: het C#-project markeert deze constructor als
intern
(commit 954951f). In Java, "internal-to-the-assembly"
vertaalt niet netjes naar package-private omdat de producenten (
WordProcessingParser
,
TableAreaParser
,
etc.) zich bevinden in
com.groupdocs.parser
, niet
com.groupdocs.parser.data
. De constructor wordt daarom behouden

public
zodat cross-package constructie nog steeds werkt.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rijen | java.lang.Iterable<java.lang.Double> | De collectie van rijhoogtes. |
|
|  | kolommen | java.lang.Iterable<java.lang.Double> | De collectie van kolombreedtes. |
|
|  | cellen | java.lang.Iterable<com.groupdocs.parser.data.PageTableAreaCell> | De collectie van cellen. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | De pagina die de tabel bevat. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied dat de tabel bevat. |
|

### getCells() {#getCells--}
```
public Collection<PageTableAreaCell> getCells()
```


Haalt de collectie van cellen op. Een eenvoudige alleen-lezen collectie van tabelcellen.


**Returns:**
java.util.Collection<com.groupdocs.parser.data.PageTableAreaCell> - Een collectie van tabelcellen

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Haalt het totale aantal rijen van de tabel op.


**Returns:**
int - Een geheel getal dat het totale aantal rijen van de tabel bevat.

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Haalt het totale aantal kolommen van de tabel op.


**Returns:**
int - Een geheel getal dat het totale aantal kolommen van de tabel bevat.

### getRowHeight(int rowIndex) {#getRowHeight-int-}
```
public double getRowHeight(int rowIndex)
```


Retourneert de rijhoogte.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rowIndex | int | De nulgebaseerde index van de rij. |
|

**Returns:**
double - Een double-waarde die de hoogte van de rij weergeeft.

### getColumnWidth(int columnIndex) {#getColumnWidth-int-}
```
public double getColumnWidth(int columnIndex)
```


Retourneert de kolombreedte.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | columnIndex | int | De nulgebaseerde index van de kolom. |
|

**Returns:**
double - Een double-waarde die de breedte van de kolom weergeeft.

### getCell(int rowIndex, int columnIndex) {#getCell-int-int-}
```
public PageTableAreaCell getCell(int rowIndex, int columnIndex)
```


Haalt de tabelcel op op basis van rij- en kolomindexen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rowIndex | int | De nulgebaseerde index van de celrij. |
|
|  | columnIndex | int | De nulgebaseerde index van de celkolom. |
|

**Returns:**
[PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) - An instance of [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) class;  null  if no cell is found.


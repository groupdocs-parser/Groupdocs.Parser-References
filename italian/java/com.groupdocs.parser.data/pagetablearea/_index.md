---
title: "PageTableArea"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta un'area tabella della pagina che è usata per rappresentare una tabella nella funzionalità di parsing tramite modello."
type: docs
weight: 22
url: /it/java/com.groupdocs.parser.data/pagetablearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTableArea extends PageArea
```

Rappresenta un'area tabella della pagina che è usata per rappresentare una tabella nella funzionalità di parsing tramite modello.

[PageTableArea](../../com.groupdocs.parser.data/pagetablearea) class is used to organize inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class in table structure.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)](#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Inizializza una nuova istanza della classe [PageTableArea](../../com.groupdocs.parser.data/pagetablearea). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getCells()](#getCells--) | Ottiene la collezione di celle. |
|
|  | [getRowCount()](#getRowCount--) | Ottiene il numero totale di righe della tabella. |
|
|  | [getColumnCount()](#getColumnCount--) | Ottiene il numero totale di colonne della tabella. |
|
|  | [getRowHeight(int rowIndex)](#getRowHeight-int-) | Restituisce l'altezza della riga. |
|
|  | [getColumnWidth(int columnIndex)](#getColumnWidth-int-) | Restituisce la larghezza della colonna. |
|
|  | [getCell(int rowIndex, int columnIndex)](#getCell-int-int-) | Ottiene la cella della tabella per gli indici di riga e colonna. |
|
### PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle) {#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)
```


Inizializza una nuova istanza della classe [PageTableArea](../../com.groupdocs.parser.data/pagetablearea).

Nota: il progetto C# segna questo costruttore come
internal
(commit 954951f). In Java, "internal-to-the-assembly"
non si traduce correttamente in package-private perché i produttori (
WordProcessingParser
,
TableAreaParser
,
ecc.) vivono in
com.groupdocs.parser
, non
com.groupdocs.parser.data
. Il costruttore è quindi mantenuto

public
in modo che la costruzione cross-package funzioni ancora.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rows | java.lang.Iterable<java.lang.Double> | La collezione delle altezze delle righe. |
|
|  | columns | java.lang.Iterable<java.lang.Double> | La collezione delle larghezze delle colonne. |
|
|  | cells | java.lang.Iterable<com.groupdocs.parser.data.PageTableAreaCell> | La collezione delle celle. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | La pagina che contiene la tabella. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare che contiene la tabella. |
|

### getCells() {#getCells--}
```
public Collection<PageTableAreaCell> getCells()
```


Ottiene la collezione delle celle. Una semplice collezione di sola lettura di celle della tabella.


**Returns:**
java.util.Collection<com.groupdocs.parser.data.PageTableAreaCell> - Una collezione di celle della tabella

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Ottiene il numero totale di righe della tabella.


**Returns:**
int - Un valore intero che contiene il numero totale di righe della tabella.

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Ottiene il numero totale di colonne della tabella.


**Returns:**
int - Un valore intero che contiene il numero totale di colonne della tabella.

### getRowHeight(int rowIndex) {#getRowHeight-int-}
```
public double getRowHeight(int rowIndex)
```


Restituisce l'altezza della riga.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rowIndex | int | L'indice basato su zero della riga. |
|

**Returns:**
double - Un valore double che rappresenta l'altezza della riga.

### getColumnWidth(int columnIndex) {#getColumnWidth-int-}
```
public double getColumnWidth(int columnIndex)
```


Restituisce la larghezza della colonna.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | columnIndex | int | L'indice basato su zero della colonna. |
|

**Returns:**
double - Un valore double che rappresenta la larghezza della colonna.

### getCell(int rowIndex, int columnIndex) {#getCell-int-int-}
```
public PageTableAreaCell getCell(int rowIndex, int columnIndex)
```


Ottiene la cella della tabella per gli indici di riga e colonna.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rowIndex | int | L'indice basato su zero della riga della cella. |
|
|  | columnIndex | int | L'indice basato su zero della colonna della cella. |
|

**Returns:**
[PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) - An instance of [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) class;  null  if no cell is found.


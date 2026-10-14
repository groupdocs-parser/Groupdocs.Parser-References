---
title: "PageTableAreaCell"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta una cella di tabella che è usata nella classe."
type: docs
weight: 23
url: /it/java/com.groupdocs.parser.data/pagetableareacell/
---
**Inheritance:**
java.lang.Object
```
public class PageTableAreaCell
```

Rappresenta una cella di tabella che è usata nella classe [PageTableArea](../../com.groupdocs.parser.data/pagetablearea).

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-) | Inizializza una nuova istanza della classe [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell). |
|
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-) | Inizializza una nuova istanza della classe [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getRowIndex()](#getRowIndex--) | Restituisce l'indice della riga. |
|
|  | [getColumnIndex()](#getColumnIndex--) | Restituisce l'indice della colonna. |
|
|  | [getRowSpan()](#getRowSpan--) | Restituisce il numero totale di righe che contengono la cella della tabella. |
|
|  | [getColumnSpan()](#getColumnSpan--) | Restituisce il numero totale di colonne che contengono la cella della tabella. |
|
|  | [getPageArea()](#getPageArea--) | Restituisce il valore della cella della tabella. |
|
|  | [getText()](#getText--) | Restituisce il valore di testo della cella della tabella. |
|
### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)
```


Inizializza una nuova istanza della classe [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rowIndex | int | L'indice basato su zero della riga. |
|
|  | columnIndex | int | L'indice basato su zero della colonna. |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | Il valore della cella della tabella. |
|

### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)
```


Inizializza una nuova istanza della classe [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rowIndex | int | L'indice basato su zero della riga. |
|
|  | columnIndex | int | L'indice basato su zero della colonna. |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | Il valore della cella della tabella. |
|
|  | rowSpan | int | Il numero totale di righe che contengono la cella della tabella. |
|
|  | columnSpan | int | Il numero totale di colonne che contengono la cella della tabella. |
|

### getRowIndex() {#getRowIndex--}
```
public int getRowIndex()
```


Restituisce l'indice della riga.


**Returns:**
int - Un indice basato su zero della prima riga che contiene la cella della tabella.

### getColumnIndex() {#getColumnIndex--}
```
public int getColumnIndex()
```


Restituisce l'indice della colonna.


**Returns:**
int - Un indice basato su zero della prima colonna che contiene la cella della tabella.

### getRowSpan() {#getRowSpan--}
```
public int getRowSpan()
```


Restituisce il numero totale di righe che contengono la cella della tabella.


**Returns:**
int - Un valore intero positivo che rappresenta il numero totale di righe che contengono la cella della tabella.

### getColumnSpan() {#getColumnSpan--}
```
public int getColumnSpan()
```


Restituisce il numero totale di colonne che contengono la cella della tabella.


**Returns:**
int - Un valore intero positivo che rappresenta il numero totale di colonne che contengono la cella della tabella.

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


Restituisce il valore della cella della tabella.


**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - Depending on cell [PageArea](../../com.groupdocs.parser.data/pagearea) property can contain any of the inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class.

### getText() {#getText--}
```
public String getText()
```


Restituisce il valore di testo della cella della tabella.


**Returns:**
java.lang.String - Una stringa che rappresenta un valore di testo della cella;  null  se la cella non contiene un valore di testo.


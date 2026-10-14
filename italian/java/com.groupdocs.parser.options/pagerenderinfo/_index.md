---
title: "PageRenderInfo"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta le informazioni su come una pagina viene renderizzata."
type: docs
weight: 30
url: /it/java/com.groupdocs.parser.options/pagerenderinfo/
---
**Inheritance:**
java.lang.Object
```
public class PageRenderInfo
```

Rappresenta le informazioni su come una pagina viene renderizzata.

Alcuni documenti (fogli di calcolo, ad esempio) non è possibile renderizzare una pagina
come un'unica immagine. Per questi documenti una pagina viene renderizzata come un insieme di tile.
Queste tile sono posizionate nella tabella rettangolare.


RowCount
e
ColumnCount
rappresentano il numero totale di righe e colonne
di questa tabella. Se la pagina del documento è renderizzata come un'unica immagine, queste proprietà sono uguali a 1.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [PageRenderInfo(int pageNumber, int rowCount, int columnCount)](#PageRenderInfo-int-int-int-) | Inizializza una nuova istanza della classe [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | Restituisce il numero della pagina. |
|
|  | [getRowCount()](#getRowCount--) | Restituisce il numero totale di righe di tile. |
|
|  | [getColumnCount()](#getColumnCount--) | Restituisce il numero totale di colonne di tile. |
|
|  | [getColumn(int tileIndex)](#getColumn-int-) | Restituisce l'indice della colonna in cui è posizionata la tile con  tileIndex . |
|
|  | [getRow(int tileIndex)](#getRow-int-) | Restituisce l'indice della riga in cui è posizionata la tile con  tileIndex . |
|
### PageRenderInfo(int pageNumber, int rowCount, int columnCount) {#PageRenderInfo-int-int-int-}
```
public PageRenderInfo(int pageNumber, int rowCount, int columnCount)
```


Inizializza una nuova istanza della classe [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pageNumber | int | Il numero della pagina (inizia da 1). |
|
|  | rowCount | int | Il numero totale di righe di tile. |
|
|  | columnCount | int | Il numero totale di colonne di tile. |
|

### getPageNumber() {#getPageNumber--}
```
public int getPageNumber()
```


Restituisce il numero della pagina.


**Returns:**
int - Il valore intero che rappresenta il numero della pagina (inizia da 1).

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Restituisce il numero totale di righe di tile.


**Returns:**
int - Il valore intero che rappresenta il numero totale di righe di tile.

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Restituisce il numero totale di colonne di tile.


**Returns:**
int - Il valore intero che rappresenta il numero totale di colonne di tile.

### getColumn(int tileIndex) {#getColumn-int-}
```
public int getColumn(int tileIndex)
```


Restituisce l'indice della colonna in cui è posizionata la tile con  tileIndex .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | tileIndex | int | L'indice a base zero della tile. |
|

**Returns:**
int - Il valore intero a base zero che rappresenta l'indice della colonna.

### getRow(int tileIndex) {#getRow-int-}
```
public int getRow(int tileIndex)
```


Restituisce l'indice della riga in cui è posizionata la tile con  tileIndex .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | tileIndex | int | L'indice a base zero della tile. |
|

**Returns:**
int - Il valore intero a base zero che rappresenta l'indice della riga.


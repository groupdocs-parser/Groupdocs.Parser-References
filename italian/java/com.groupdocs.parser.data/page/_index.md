---
title: "Page"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta le informazioni della pagina del documento come l'indice della pagina e le dimensioni della pagina."
type: docs
weight: 16
url: /it/java/com.groupdocs.parser.data/page/
---
**Inheritance:**
java.lang.Object
```
public class Page
```

Rappresenta le informazioni della pagina del documento, come l'indice della pagina e le dimensioni della pagina. Viene utilizzato per rappresentare la pagina che contiene gli eredi della classe [PageArea](../../com.groupdocs.parser.data/pagearea) nella funzionalità di parsing tramite modello.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [Page(int index, Size size)](#Page-int-com.groupdocs.parser.data.Size-) | Inizializza una nuova istanza della classe [Page](../../com.groupdocs.parser.data/page). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getIndex()](#getIndex--) | Restituisce l'indice della pagina. |
|
|  | [getSize()](#getSize--) | Restituisce le dimensioni della pagina. |
|
### Page(int index, Size size) {#Page-int-com.groupdocs.parser.data.Size-}
```
public Page(int index, Size size)
```


Inizializza una nuova istanza della classe [Page](../../com.groupdocs.parser.data/page).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | indice | int | L'indice della pagina. |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | Le dimensioni della pagina. |
|

### getIndex() {#getIndex--}
```
public int getIndex()
```


Restituisce l'indice della pagina.


**Returns:**
int - Un indice basato su zero della pagina.

### getSize() {#getSize--}
```
public Size getSize()
```


Restituisce le dimensioni della pagina.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the page.


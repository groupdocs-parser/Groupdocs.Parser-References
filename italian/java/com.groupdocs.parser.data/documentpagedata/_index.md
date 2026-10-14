---
title: "DocumentPageData"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta i dati della pagina del documento."
type: docs
weight: 12
url: /it/java/com.groupdocs.parser.data/documentpagedata/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.DocumentData](../../com.groupdocs.parser.data/documentdata)
```
public class DocumentPageData extends DocumentData
```

Rappresenta i dati della pagina del documento. È costituito da oggetti [FieldData](../../com.groupdocs.parser.data/fielddata) che contengono i dati dei campi dalla pagina del documento.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [DocumentPageData(Iterable<FieldData> fields, int pageIndex)](#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-) | Inizializza una nuova istanza della classe [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getPageIndex()](#getPageIndex--) | Restituisce l'indice della pagina. |
|
### DocumentPageData(Iterable<FieldData> fields, int pageIndex) {#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-}
```
public DocumentPageData(Iterable<FieldData> fields, int pageIndex)
```


Inizializza una nuova istanza della classe [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | campi | java.lang.Iterable<com.groupdocs.parser.data.FieldData> | La collezione dei dati dei campi. |
|
|  | pageIndex | int | L'indice della pagina basato su zero. |
|

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Restituisce l'indice della pagina.


**Returns:**
int - Un indice basato su zero della pagina.


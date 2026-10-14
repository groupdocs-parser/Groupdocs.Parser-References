---
title: "PageGroupArea"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta un gruppo di aree della pagina che è usato per raggruppare diversi tipi di blocchi della pagina del documento nella funzionalità di parsing tramite modello."
type: docs
weight: 19
url: /it/java/com.groupdocs.parser.data/pagegrouparea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageGroupArea extends PageArea
```

Rappresenta un gruppo di aree della pagina che è usato per raggruppare diversi tipi di blocchi della pagina del documento nella funzionalità di parsing tramite modello.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [PageGroupArea(Iterable<PageArea> areas, Page page)](#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-) | Inizializza una nuova istanza della classe [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getAreas()](#getAreas--) | Restituisce la collezione di aree di pagina raggruppate. |
|
### PageGroupArea(Iterable<PageArea> areas, Page page) {#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-}
```
public PageGroupArea(Iterable<PageArea> areas, Page page)
```


Inizializza una nuova istanza della classe [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | areas | java.lang.Iterable<com.groupdocs.parser.data.PageArea> | La collezione di aree di pagina da raggruppare. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | La pagina che contiene l'area. |
|

### getAreas() {#getAreas--}
```
public Iterable<PageArea> getAreas()
```


Restituisce la collezione di aree di pagina raggruppate.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageArea> - Una collezione di oggetti [PageArea](../../com.groupdocs.parser.data/pagearea).


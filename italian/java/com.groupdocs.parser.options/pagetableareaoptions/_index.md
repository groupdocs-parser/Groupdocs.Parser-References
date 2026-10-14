---
title: "PageTableAreaOptions"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce le opzioni utilizzate per l'estrazione delle aree di tabella della pagina."
type: docs
weight: 31
url: /it/java/com.groupdocs.parser.options/pagetableareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTableAreaOptions extends PageAreaOptions
```

Fornisce le opzioni utilizzate per l'estrazione delle aree di tabella della pagina.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [PageTableAreaOptions(TemplateTableLayout tableLayout)](#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-) | Inizializza una nuova istanza della classe [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions). |
|
|  | [PageTableAreaOptions(Rectangle rectangle)](#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-) | Inizializza una nuova istanza della classe [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) con un rettangolo di ricerca e nessun layout fisso. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getTableLayout()](#getTableLayout--) | Ottiene il layout della tabella che definisce la tabella in una pagina. |
|
### PageTableAreaOptions(TemplateTableLayout tableLayout) {#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-}
```
public PageTableAreaOptions(TemplateTableLayout tableLayout)
```


Inizializza una nuova istanza della classe [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | tableLayout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Il layout della tabella che definisce la tabella in una pagina. |
|

### PageTableAreaOptions(Rectangle rectangle) {#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageTableAreaOptions(Rectangle rectangle)
```


Inizializza una nuova istanza della classe [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) con un rettangolo di ricerca e nessun layout fisso.

Utile per limitare le tabelle auto-rilevate a una regione della pagina. Riflette il C#

new PageTableAreaOptions(null) { Rectangle = ... }
modello.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare nella pagina dove le tabelle devono essere rilevate; passa null per cercare l'intera pagina. |
|

### getTableLayout() {#getTableLayout--}
```
public TemplateTableLayout getTableLayout()
```


Ottiene il layout della tabella che definisce la tabella in una pagina.


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instane of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class.


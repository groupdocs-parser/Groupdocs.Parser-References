---
title: "PageArea"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta una classe base astratta per le aree della pagina che sono usate per rappresentare blocchi sulla pagina del documento nella funzionalità di parsing tramite modello."
type: docs
weight: 17
url: /it/java/com.groupdocs.parser.data/pagearea/
---
**Inheritance:**
java.lang.Object
```
public abstract class PageArea
```

Rappresenta una classe base astratta per le aree della pagina che sono usate per rappresentare blocchi sulla pagina del documento nella funzionalità di parsing tramite modello.

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Restituisce l'area rettangolare. |
|
|  | [getPage()](#getPage--) | Restituisce le informazioni della pagina del documento, come l'indice della pagina e le dimensioni della pagina. |
|
### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Restituisce l'area rettangolare.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area of the page that contains the page area.

### getPage() {#getPage--}
```
public Page getPage()
```


Restituisce le informazioni della pagina del documento, come l'indice della pagina e le dimensioni della pagina.


**Returns:**
[Page](../../com.groupdocs.parser.data/page) - An instance of [Page](../../com.groupdocs.parser.data/page) class that represents the page that contains the page area.


---
title: "PageAreaOptions"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce le opzioni utilizzate per l'estrazione delle aree di pagina."
type: docs
weight: 28
url: /it/java/com.groupdocs.parser.options/pageareaoptions/
---
**Inheritance:**
java.lang.Object
```
public class PageAreaOptions
```

Fornisce le opzioni utilizzate per l'estrazione delle aree di pagina.

Un'istanza della classe [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) è usata come parametro in [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-)
e nei metodi [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-). Vedi gli esempi d'uso lì.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [PageAreaOptions(Rectangle rectangle)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-) | Inizializza una nuova istanza della classe [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) con la dimensione del bordo ignorato. |
|
|  | [PageAreaOptions(Rectangle rectangle, double rectangleTolerance)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-) | Inizializza una nuova istanza della classe [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Restituisce l'area rettangolare che contiene le aree della pagina. |
|
|  | [getRectangleTolerance()](#getRectangleTolerance--) | Restituisce la dimensione del bordo che viene ignorata quando catturata dall'area rettangolare. |
|
### PageAreaOptions(Rectangle rectangle) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageAreaOptions(Rectangle rectangle)
```


Inizializza una nuova istanza della classe [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) con la dimensione del bordo ignorato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare che contiene le aree della pagina. |
|

### PageAreaOptions(Rectangle rectangle, double rectangleTolerance) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-}
```
public PageAreaOptions(Rectangle rectangle, double rectangleTolerance)
```


Inizializza una nuova istanza della classe [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare che contiene le aree della pagina. |
|
|  | rectangleTolerance | double | La dimensione del bordo che viene ignorata quando catturata dall'area rettangolare. È misurata come frazione dell'altezza di un elemento di testo. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Restituisce l'area rettangolare che contiene le aree della pagina.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


Restituisce la dimensione del bordo che viene ignorata quando catturata dall'area rettangolare. È misurata come frazione dell'altezza di un elemento di testo.


**Returns:**
double - Il valore double da 0 (nessun bordo) a 1 (ignora l'intero elemento).


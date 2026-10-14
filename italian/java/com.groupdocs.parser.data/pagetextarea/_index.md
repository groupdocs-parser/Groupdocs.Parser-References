---
title: "PageTextArea"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta un'area di testo della pagina che è usata per rappresentare un valore di testo nella funzionalità di parsing tramite modello o di parsing di modulo."
type: docs
weight: 24
url: /it/java/com.groupdocs.parser.data/pagetextarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTextArea extends PageArea
```

Rappresenta un'area di testo della pagina che è usata per rappresentare un valore di testo nella funzionalità di parsing tramite modello o di parsing di modulo.

Un'istanza della classe [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) è usata come valore di ritorno dei seguenti metodi:

* [Parser.getTextAreas()](../../com.groupdocs.parser/parser#getTextAreas--)
* [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-)
* [Parser.getTextAreas(int)](../../com.groupdocs.parser/parser#getTextAreas-int-)
* [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-)

Anche un'istanza della classe [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) è usata come valore della proprietà [PageArea](../../com.groupdocs.parser.data/pagearea).
\*

Vedi gli esempi di utilizzo lì.

L'area di testo può essere singola o composita. Nel primo caso contiene un testo delimitato da un'area rettangolare.
Nel secondo caso contiene altre aree di testo; le proprietà di testo e di tabella sono calcolate dalle aree di testo figlie.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [PageTextArea(String text, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Inizializza una nuova istanza della classe [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
|  | [PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Inizializza una nuova istanza della classe [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
|  | [PageTextArea(Iterable<PageTextArea> areas, Page page)](#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-) | Inizializza una nuova istanza della classe [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getText()](#getText--) | Restituisce il testo. |
|
|  | [getBaseLine()](#getBaseLine--) | Ottiene la linea di base. |
|
|  | [getTextStyle()](#getTextStyle--) | Ottiene lo stile del testo, come la dimensione del carattere, il nome del carattere e così via. |
|
|  | [getAreas()](#getAreas--) | Ottiene la collezione delle aree di pagina di testo figlie. |
|
### PageTextArea(String text, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Page page, Rectangle rectangle)
```


Inizializza una nuova istanza della classe [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | testo | java.lang.String | Il valore del testo. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | La pagina che contiene l'area di testo. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare che contiene l'area di testo. |
|

### PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)
```


Inizializza una nuova istanza della classe [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | testo | java.lang.String | Il valore del testo. |
|
|  | baseLine | java.lang.Double | La linea di base del testo. |
|
|  | textStyle | [TextStyle](../../com.groupdocs.parser.data/textstyle) | Lo stile del testo. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | La pagina che contiene l'area di testo. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare che contiene l'area di testo. |
|

### PageTextArea(Iterable<PageTextArea> areas, Page page) {#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-}
```
public PageTextArea(Iterable<PageTextArea> areas, Page page)
```


Inizializza una nuova istanza della classe [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | areas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | La collezione delle aree di pagina di testo figlie. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | La pagina che contiene l'area di testo. |
|

### getText() {#getText--}
```
public String getText()
```


Restituisce il testo.


**Returns:**
java.lang.String - Un valore stringa che rappresenta un valore dell'area di pagina di testo.

### getBaseLine() {#getBaseLine--}
```
public double getBaseLine()
```


Ottiene la linea di base.


**Returns:**
double - Un valore double che rappresenta la linea di base.

### getTextStyle() {#getTextStyle--}
```
public TextStyle getTextStyle()
```


Ottiene lo stile del testo, come la dimensione del carattere, il nome del carattere e così via.


**Returns:**
[TextStyle](../../com.groupdocs.parser.data/textstyle) - An instance of [TextStyle](../../com.groupdocs.parser.data/textstyle) class that represents the text style.

### getAreas() {#getAreas--}
```
public List<PageTextArea> getAreas()
```


Ottiene la collezione delle aree di pagina di testo figlie.


**Returns:**
java.util.List<com.groupdocs.parser.data.PageTextArea> - Una collezione di aree di pagina di testo figlie; vuota se l'area di pagina di testo non ha figli.


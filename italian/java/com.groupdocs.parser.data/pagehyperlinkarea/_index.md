---
title: "PageHyperlinkArea"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta un'area della pagina che è usata per rappresentare un collegamento ipertestuale nella pagina."
type: docs
weight: 20
url: /it/java/com.groupdocs.parser.data/pagehyperlinkarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageHyperlinkArea extends PageArea
```

Rappresenta un'area della pagina che è usata per rappresentare un collegamento ipertestuale nella pagina.

Un'istanza della classe [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) è usata come valore di ritorno dei seguenti metodi:

* [Parser.getHyperlinks()](../../com.groupdocs.parser/parser#getHyperlinks--)
* [Parser.getHyperlinks(PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-PageAreaOptions-)
* [Parser.getHyperlinks(int)](../../com.groupdocs.parser/parser#getHyperlinks-int-)
* [Parser.getHyperlinks(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-int--PageAreaOptions-)

Vedi gli esempi di utilizzo lì.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)](#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Inizializza una nuova istanza della classe [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getText()](#getText--) | Ottiene il testo del collegamento ipertestuale. |
|
|  | [getUrl()](#getUrl--) | Ottiene l'URL del collegamento ipertestuale. |
|
### PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle) {#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)
```


Inizializza una nuova istanza della classe [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | testo | java.lang.String | Il testo del collegamento ipertestuale. |
|
|  | url | java.lang.String | L'URL del collegamento ipertestuale. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | La pagina che contiene il collegamento ipertestuale. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare che contiene il collegamento ipertestuale. |
|

### getText() {#getText--}
```
public String getText()
```


Ottiene il testo del collegamento ipertestuale.


**Returns:**
java.lang.String - Un valore stringa che rappresenta il testo del collegamento ipertestuale.

### getUrl() {#getUrl--}
```
public String getUrl()
```


Ottiene l'URL del collegamento ipertestuale.


**Returns:**
java.lang.String - Un valore stringa che rappresenta l'URL del collegamento ipertestuale.


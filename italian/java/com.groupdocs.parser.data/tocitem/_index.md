---
title: "TocItem"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta l'elemento utilizzato nella funzionalità di estrazione dell'indice."
type: docs
weight: 31
url: /it/java/com.groupdocs.parser.data/tocitem/
---
**Inheritance:**
java.lang.Object
```
public class TocItem
```

Rappresenta l'elemento utilizzato nella funzionalità di estrazione dell'indice.

Un'istanza della classe [TocItem](../../com.groupdocs.parser.data/tocitem) è usata come valore di ritorno del metodo [Parser.getToc()](../../com.groupdocs.parser/parser#getToc--) . Vedi gli esempi d'uso lì.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [TocItem(int depth, String text, Integer pageIndex)](#TocItem-int-java.lang.String-java.lang.Integer-) | Inizializza una nuova istanza della classe TocItem. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getDepth()](#getDepth--) | Restituisce il livello di profondità. |
|
|  | [getText()](#getText--) | Restituisce il testo. |
|
|  | [getPageIndex()](#getPageIndex--) | Restituisce l'indice della pagina. |
|
|  | [extractText()](#extractText--) | Estrae un testo dal documento a cui fa riferimento l'oggetto TocItem. |
|
### TocItem(int depth, String text, Integer pageIndex) {#TocItem-int-java.lang.String-java.lang.Integer-}
```
public TocItem(int depth, String text, Integer pageIndex)
```


Inizializza una nuova istanza della classe TocItem.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | profondità | int | Il livello di profondità dell'elemento. |
|
|  | testo | java.lang.String | Il testo dell'elemento. |
|
|  | pageIndex | java.lang.Integer | L'indice della pagina a cui fa riferimento l'elemento |
|

### getDepth() {#getDepth--}
```
public int getDepth()
```


Restituisce il livello di profondità.


**Returns:**
int - Un valore intero che rappresenta il livello di profondità dell'elemento.

### getText() {#getText--}
```
public String getText()
```


Restituisce il testo.


**Returns:**
java.lang.String - Un valore stringa che rappresenta il testo dell'elemento.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Restituisce l'indice della pagina.


**Returns:**
java.lang.Integer - Un valore intero che rappresenta l'indice della pagina a cui fa riferimento l'elemento;  null  se non è impostato.

### extractText() {#extractText--}
```
public TextReader extractText()
```


Estrae un testo dal documento a cui fa riferimento l'oggetto TocItem.

Il seguente esempio su come estrarre un testo tramite un elemento del sommario:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleDocxWithToc)) {
     // Get table of contents
     Iterable tocItems = parser.getToc();

     // Check if toc extraction is supported
     if (tocItems == null) {
         System.out.println("Table of contents extraction isn't supported");
     }

     // Iterate over items
     for (TocItem tocItem : tocItems) {
         // Print the text of the chapter
         try (TextReader reader = tocItem.extractText()) {
             System.out.println("----");
             System.out.println(reader.readToEnd());
         }
     }
 }
 
````



**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text.


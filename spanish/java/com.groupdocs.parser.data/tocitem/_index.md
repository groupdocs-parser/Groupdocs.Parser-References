---
title: "TocItem"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa el elemento que se utiliza en la funcionalidad de extracción del índice."
type: docs
weight: 31
url: /es/java/com.groupdocs.parser.data/tocitem/
---
**Inheritance:**
java.lang.Object
```
public class TocItem
```

Representa el elemento que se utiliza en la funcionalidad de extracción del índice.

Una instancia de la clase [TocItem](../../com.groupdocs.parser.data/tocitem) se utiliza como valor de retorno del método [Parser.getToc()](../../com.groupdocs.parser/parser#getToc--). Consulte los ejemplos de uso allí.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [TocItem(int depth, String text, Integer pageIndex)](#TocItem-int-java.lang.String-java.lang.Integer-) | Inicializa una nueva instancia de la clase TocItem. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getDepth()](#getDepth--) | Obtiene el nivel de profundidad. |
|
|  | [getText()](#getText--) | Obtiene el texto. |
|
|  | [getPageIndex()](#getPageIndex--) | Obtiene el índice de página. |
|
|  | [extractText()](#extractText--) | Extrae un texto del documento al que se refiere el objeto TocItem. |
|
### TocItem(int depth, String text, Integer pageIndex) {#TocItem-int-java.lang.String-java.lang.Integer-}
```
public TocItem(int depth, String text, Integer pageIndex)
```


Inicializa una nueva instancia de la clase TocItem.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | profundidad | int | El nivel de profundidad del elemento. |
|
|  | texto | java.lang.String | El texto del elemento. |
|
|  | pageIndex | java.lang.Integer | El índice de la página referenciada por el elemento |
|

### getDepth() {#getDepth--}
```
public int getDepth()
```


Obtiene el nivel de profundidad.


**Returns:**
int - Un valor entero que representa el nivel de profundidad del elemento.

### getText() {#getText--}
```
public String getText()
```


Obtiene el texto.


**Returns:**
java.lang.String - Un valor de cadena que representa el texto del elemento.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Obtiene el índice de página.


**Returns:**
java.lang.Integer - Un valor entero que representa el índice de la página referenciada por el elemento;  null  si no está establecido.

### extractText() {#extractText--}
```
public TextReader extractText()
```


Extrae un texto del documento al que se refiere el objeto TocItem.

El siguiente ejemplo muestra cómo extraer un texto mediante un elemento de la tabla de contenido:

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


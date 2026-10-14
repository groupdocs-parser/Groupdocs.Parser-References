---
title: "SearchResult"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa el resultado de búsqueda en la funcionalidad de búsqueda."
type: docs
weight: 27
url: /es/java/com.groupdocs.parser.data/searchresult/
---
**Inheritance:**
java.lang.Object
```
public class SearchResult
```

Representa el resultado de búsqueda en la funcionalidad de búsqueda.

Una instancia de la clase SearchResult se usa como valor de retorno de [Parser.search(String)](../../com.groupdocs.parser/parser#search-String-)
y los métodos [Parser.search(String, com.groupdocs.parser.options.SearchOptions)](../../com.groupdocs.parser/parser#search-String--com.groupdocs.parser.options.SearchOptions-). Vea los ejemplos de uso allí.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)](#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-) | Inicializa una nueva instancia de la clase [SearchResult](../../com.groupdocs.parser.data/searchresult). |
|
|  | [SearchResult(int position, String text, Integer pageIndex)](#SearchResult-int-java.lang.String-java.lang.Integer-) | Inicializa una nueva instancia de la clase [SearchResult](../../com.groupdocs.parser.data/searchresult). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getPosition()](#getPosition--) | Obtiene la posición en el texto del documento. |
|
|  | [getText()](#getText--) | Obtiene el texto. |
|
|  | [getPageIndex()](#getPageIndex--) | Obtiene el índice de página donde se encuentra el texto. |
|
|  | [getLeftHighlightItem()](#getLeftHighlightItem--) | Obtiene el resaltado izquierdo. |
|
|  | [getRightHighlightItem()](#getRightHighlightItem--) | Obtiene el resaltado derecho. |
|
### SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem) {#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-}
```
public SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)
```


Inicializa una nueva instancia de la clase [SearchResult](../../com.groupdocs.parser.data/searchresult).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | posición | int | La posición en el texto del documento. |
|
|  | texto | java.lang.String | El texto encontrado. |
|
|  | pageIndex | java.lang.Integer | El índice de página donde se encuentra el texto. |
|
|  | leftHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | El resaltado izquierdo. |
|
|  | rightHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | El resaltado derecho. |
|

### SearchResult(int position, String text, Integer pageIndex) {#SearchResult-int-java.lang.String-java.lang.Integer-}
```
public SearchResult(int position, String text, Integer pageIndex)
```


Inicializa una nueva instancia de la clase [SearchResult](../../com.groupdocs.parser.data/searchresult).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | posición | int | La posición en el texto del documento. |
|
|  | texto | java.lang.String | El texto encontrado. |
|
|  | pageIndex | java.lang.Integer | El índice de página donde se encuentra el texto. |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


Obtiene la posición en el texto del documento.


**Returns:**
int - Un índice basado en cero de la posición inicial del resultado de búsqueda.

### getText() {#getText--}
```
public String getText()
```


Obtiene el texto.


**Returns:**
java.lang.String - Un valor de cadena que representa el texto encontrado.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Obtiene el índice de página donde se encuentra el texto.


**Returns:**
java.lang.Integer - Un índice basado en cero de la página donde se encuentra el texto;  null  si la búsqueda se realiza en todo el texto del documento.

### getLeftHighlightItem() {#getLeftHighlightItem--}
```
public HighlightItem getLeftHighlightItem()
```


Obtiene el resaltado izquierdo.


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

### getRightHighlightItem() {#getRightHighlightItem--}
```
public HighlightItem getRightHighlightItem()
```


Obtiene el resaltado derecho.


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.


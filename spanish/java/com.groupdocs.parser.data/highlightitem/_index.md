---
title: "HighlightItem"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa un resaltado de una parte del texto que normalmente se usa para explicar el contexto del texto encontrado en la funcionalidad de búsqueda."
type: docs
weight: 14
url: /es/java/com.groupdocs.parser.data/highlightitem/
---
**Inheritance:**
java.lang.Object
```
public class HighlightItem
```

Representa un resaltado, una parte del texto que normalmente se usa para explicar el contexto del texto encontrado en la funcionalidad de búsqueda.

Una instancia de la clase [HighlightItem](../../com.groupdocs.parser.data/highlightitem) se usa como valor de retorno del método [Parser.getHighlight(int, boolean, com.groupdocs.parser.options.HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--com.groupdocs.parser.options.HighlightOptions-),
[SearchResult.getLeftHighlightItem()](../../com.groupdocs.parser.data/searchresult#getLeftHighlightItem--) and [SearchResult.getRightHighlightItem()](../../com.groupdocs.parser.data/searchresult#getRightHighlightItem--) properties. See the usage examples there.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [HighlightItem(int position, String text)](#HighlightItem-int-java.lang.String-) | Inicializa una nueva instancia de la clase [HighlightItem](../../com.groupdocs.parser.data/highlightitem). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getPosition()](#getPosition--) | Obtiene la posición en el texto del documento. |
|
|  | [getText()](#getText--) | Obtiene el texto del resaltado. |
|
### HighlightItem(int position, String text) {#HighlightItem-int-java.lang.String-}
```
public HighlightItem(int position, String text)
```


Inicializa una nueva instancia de la clase [HighlightItem](../../com.groupdocs.parser.data/highlightitem).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | posición | int | La posición en el texto del documento. |
|
|  | texto | java.lang.String | El texto del resaltado. |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


Obtiene la posición en el texto del documento.


**Returns:**
int - Un índice basado en cero de la posición inicial del resaltado.

### getText() {#getText--}
```
public String getText()
```


Obtiene el texto del resaltado.


**Returns:**
java.lang.String - Un valor de cadena que representa el texto del resaltado.


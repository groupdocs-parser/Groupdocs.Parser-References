---
title: "OcrEventHandler"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona un controlador para eventos OCR."
type: docs
weight: 26
url: /es/java/com.groupdocs.parser.options/ocreventhandler/
---
**Inheritance:**
java.lang.Object
```
public class OcrEventHandler
```

Proporciona un controlador para eventos OCR.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [OcrEventHandler()](#OcrEventHandler--) | Inicializa una nueva instancia de la clase [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getWarnings()](#getWarnings--) | Obtiene una lista de mensajes de advertencia. |
|
|  | [hasWarnings()](#hasWarnings--) | Obtiene el valor que indica si la lista de advertencias no está vacía. |
|
|  | [getWarnings(int pageIndex)](#getWarnings-int-) | Devuelve una lista de mensajes de advertencia para la página con pageIndex. |
|
|  | [onWarnings(int pageIndex, Iterable<String> warnings)](#onWarnings-int-java.lang.Iterable-java.lang.String--) | Establece los mensajes de advertencia para la página. |
|
### OcrEventHandler() {#OcrEventHandler--}
```
public OcrEventHandler()
```


Inicializa una nueva instancia de la clase [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


### getWarnings() {#getWarnings--}
```
public List<String> getWarnings()
```


Obtiene una lista de mensajes de advertencia.


**Returns:**
java.util.List<java.lang.String> - Una lista de mensajes de advertencia para todas las páginas.

### hasWarnings() {#hasWarnings--}
```
public boolean hasWarnings()
```


Obtiene el valor que indica si la lista de advertencias no está vacía.


**Returns:**
boolean -  true  si la lista de advertencias no está vacía; de lo contrario,  false .

### getWarnings(int pageIndex) {#getWarnings-int-}
```
public List<String> getWarnings(int pageIndex)
```


Devuelve una lista de mensajes de advertencia para la página con pageIndex.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | pageIndex | int | El índice de página basado en cero. |
|

**Returns:**
java.util.List<java.lang.String> - Una lista de mensajes de advertencia para la página; lista vacía si no hay mensajes de advertencia para la página.

### onWarnings(int pageIndex, Iterable<String> warnings) {#onWarnings-int-java.lang.Iterable-java.lang.String--}
```
public void onWarnings(int pageIndex, Iterable<String> warnings)
```


Establece los mensajes de advertencia para la página.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | pageIndex | int | El índice de página basado en cero. |
|
|  | warnings | java.lang.Iterable<java.lang.String> | La lista de mensajes de advertencia para la página. |
|


---
title: "Page"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa la información de la página del documento, como el índice de página y el tamaño de página."
type: docs
weight: 16
url: /es/java/com.groupdocs.parser.data/page/
---
**Inheritance:**
java.lang.Object
```
public class Page
```

Representa la información de la página del documento, como el índice de página y el tamaño de página. Se utiliza para representar la página que contiene herederos de la clase [PageArea](../../com.groupdocs.parser.data/pagearea) en la funcionalidad de análisis por plantilla.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [Page(int index, Size size)](#Page-int-com.groupdocs.parser.data.Size-) | Inicializa una nueva instancia de la clase [Page](../../com.groupdocs.parser.data/page). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getIndex()](#getIndex--) | Obtiene el índice de página. |
|
|  | [getSize()](#getSize--) | Obtiene el tamaño de la página. |
|
### Page(int index, Size size) {#Page-int-com.groupdocs.parser.data.Size-}
```
public Page(int index, Size size)
```


Inicializa una nueva instancia de la clase [Page](../../com.groupdocs.parser.data/page).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | índice | int | El índice de la página. |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | El tamaño de la página. |
|

### getIndex() {#getIndex--}
```
public int getIndex()
```


Obtiene el índice de página.


**Returns:**
int - Un índice basado en cero de la página.

### getSize() {#getSize--}
```
public Size getSize()
```


Obtiene el tamaño de la página.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the page.


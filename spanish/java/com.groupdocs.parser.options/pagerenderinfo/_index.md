---
title: "PageRenderInfo"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa la información de cómo se renderiza una página."
type: docs
weight: 30
url: /es/java/com.groupdocs.parser.options/pagerenderinfo/
---
**Inheritance:**
java.lang.Object
```
public class PageRenderInfo
```

Representa la información de cómo se renderiza una página.

Algunos documentos (hojas de cálculo, por ejemplo) no pueden renderizar una página
como una sola imagen. Para esos documentos, una página se renderiza como un conjunto de mosaicos.
Estos mosaicos se colocan en la tabla rectangular.


RowCount
y
ColumnCount
representan el número total de filas y columnas
de esta tabla. Si la página del documento se renderiza como una sola imagen, estas propiedades son iguales a 1.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [PageRenderInfo(int pageNumber, int rowCount, int columnCount)](#PageRenderInfo-int-int-int-) | Inicializa una nueva instancia de la clase [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | Obtiene el número de página. |
|
|  | [getRowCount()](#getRowCount--) | Obtenga el número total de filas de mosaicos. |
|
|  | [getColumnCount()](#getColumnCount--) | Obtenga el número total de columnas de mosaicos. |
|
|  | [getColumn(int tileIndex)](#getColumn-int-) | Devuelve el índice de la columna donde se coloca el mosaico con  tileIndex . |
|
|  | [getRow(int tileIndex)](#getRow-int-) | Devuelve el índice de la fila donde se coloca el mosaico con  tileIndex . |
|
### PageRenderInfo(int pageNumber, int rowCount, int columnCount) {#PageRenderInfo-int-int-int-}
```
public PageRenderInfo(int pageNumber, int rowCount, int columnCount)
```


Inicializa una nueva instancia de la clase [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | pageNumber | int | El número de la página (comienza en 1). |
|
|  | rowCount | int | El número total de filas de mosaicos. |
|
|  | columnCount | int | El número total de columnas de mosaicos. |
|

### getPageNumber() {#getPageNumber--}
```
public int getPageNumber()
```


Obtiene el número de página.


**Returns:**
int - El valor entero que representa el número de página (comienza en 1).

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Obtenga el número total de filas de mosaicos.


**Returns:**
int - El valor entero que representa el número total de filas de mosaicos.

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Obtenga el número total de columnas de mosaicos.


**Returns:**
int - El valor entero que representa el número total de columnas de mosaicos.

### getColumn(int tileIndex) {#getColumn-int-}
```
public int getColumn(int tileIndex)
```


Devuelve el índice de la columna donde se coloca el mosaico con  tileIndex .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | tileIndex | int | El índice basado en cero del mosaico. |
|

**Returns:**
int - El valor entero basado en cero que representa el índice de columna.

### getRow(int tileIndex) {#getRow-int-}
```
public int getRow(int tileIndex)
```


Devuelve el índice de la fila donde se coloca el mosaico con  tileIndex .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | tileIndex | int | El índice basado en cero del mosaico. |
|

**Returns:**
int - El valor entero basado en cero que representa el índice de fila.


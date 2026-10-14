---
title: "PageTableAreaCell"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa una celda de tabla que se usa en la clase."
type: docs
weight: 23
url: /es/java/com.groupdocs.parser.data/pagetableareacell/
---
**Inheritance:**
java.lang.Object
```
public class PageTableAreaCell
```

Representa una celda de tabla que se usa en la clase [PageTableArea](../../com.groupdocs.parser.data/pagetablearea).

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-) | Inicializa una nueva instancia de la clase [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell). |
|
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-) | Inicializa una nueva instancia de la clase [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getRowIndex()](#getRowIndex--) | Obtiene el índice de fila. |
|
|  | [getColumnIndex()](#getColumnIndex--) | Obtiene el índice de columna. |
|
|  | [getRowSpan()](#getRowSpan--) | Obtiene el número total de filas que contiene la celda de tabla. |
|
|  | [getColumnSpan()](#getColumnSpan--) | Obtiene el número total de columnas que contiene la celda de tabla. |
|
|  | [getPageArea()](#getPageArea--) | Obtiene el valor de la celda de tabla. |
|
|  | [getText()](#getText--) | Obtiene el valor de texto de la celda de tabla. |
|
### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)
```


Inicializa una nueva instancia de la clase [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rowIndex | int | El índice basado en cero de la fila. |
|
|  | columnIndex | int | El índice basado en cero de la columna. |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | El valor de la celda de tabla. |
|

### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)
```


Inicializa una nueva instancia de la clase [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rowIndex | int | El índice basado en cero de la fila. |
|
|  | columnIndex | int | El índice basado en cero de la columna. |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | El valor de la celda de tabla. |
|
|  | rowSpan | int | El número total de filas que contiene la celda de tabla. |
|
|  | columnSpan | int | El número total de columnas que contiene la celda de tabla. |
|

### getRowIndex() {#getRowIndex--}
```
public int getRowIndex()
```


Obtiene el índice de fila.


**Returns:**
int - Un índice basado en cero de la primera fila que contiene la celda de tabla.

### getColumnIndex() {#getColumnIndex--}
```
public int getColumnIndex()
```


Obtiene el índice de columna.


**Returns:**
int - Un índice basado en cero de la primera columna que contiene la celda de tabla.

### getRowSpan() {#getRowSpan--}
```
public int getRowSpan()
```


Obtiene el número total de filas que contiene la celda de tabla.


**Returns:**
int - Un valor entero positivo que representa el número total de filas que contiene la celda de tabla.

### getColumnSpan() {#getColumnSpan--}
```
public int getColumnSpan()
```


Obtiene el número total de columnas que contiene la celda de tabla.


**Returns:**
int - Un valor entero positivo que representa el número total de columnas que contiene la celda de tabla.

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


Obtiene el valor de la celda de tabla.


**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - Depending on cell [PageArea](../../com.groupdocs.parser.data/pagearea) property can contain any of the inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class.

### getText() {#getText--}
```
public String getText()
```


Obtiene el valor de texto de la celda de tabla.


**Returns:**
java.lang.String - Una cadena que representa un valor de texto de la celda;  null  si la celda no contiene un valor de texto.


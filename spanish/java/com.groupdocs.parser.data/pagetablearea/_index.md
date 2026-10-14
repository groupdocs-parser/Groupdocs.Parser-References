---
title: "PageTableArea"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa un área de tabla de página que se utiliza para representar una tabla en la funcionalidad de análisis mediante plantillas."
type: docs
weight: 22
url: /es/java/com.groupdocs.parser.data/pagetablearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTableArea extends PageArea
```

Representa un área de tabla de página que se utiliza para representar una tabla en la funcionalidad de análisis mediante plantillas.

[PageTableArea](../../com.groupdocs.parser.data/pagetablearea) class is used to organize inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class in table structure.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)](#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Inicializa una nueva instancia de la clase [PageTableArea](../../com.groupdocs.parser.data/pagetablearea). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getCells()](#getCells--) | Obtiene la colección de celdas. |
|
|  | [getRowCount()](#getRowCount--) | Obtiene el número total de filas de la tabla. |
|
|  | [getColumnCount()](#getColumnCount--) | Obtiene el número total de columnas de la tabla. |
|
|  | [getRowHeight(int rowIndex)](#getRowHeight-int-) | Devuelve la altura de la fila. |
|
|  | [getColumnWidth(int columnIndex)](#getColumnWidth-int-) | Devuelve el ancho de la columna. |
|
|  | [getCell(int rowIndex, int columnIndex)](#getCell-int-int-) | Obtiene la celda de la tabla por índices de fila y columna. |
|
### PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle) {#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)
```


Inicializa una nueva instancia de la clase [PageTableArea](../../com.groupdocs.parser.data/pagetablearea).

Nota: el proyecto C# marca este constructor como
interno
(commit 954951f). En Java, "internal-to-the-assembly"
no se traduce limpiamente a package-private porque los productores (
WordProcessingParser
,
TableAreaParser
,
etc.) viven en
com.groupdocs.parser
, no
com.groupdocs.parser.data
. Por lo tanto, el constructor se mantiene

público
para que la construcción entre paquetes siga funcionando.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filas | java.lang.Iterable<java.lang.Double> | La colección de alturas de fila. |
|
|  | columnas | java.lang.Iterable<java.lang.Double> | La colección de anchos de columna. |
|
|  | celdas | java.lang.Iterable<com.groupdocs.parser.data.PageTableAreaCell> | La colección de celdas. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | La página que contiene la tabla. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular que contiene la tabla. |
|

### getCells() {#getCells--}
```
public Collection<PageTableAreaCell> getCells()
```


Obtiene la colección de celdas. Una colección simple de solo lectura de celdas de tabla.


**Returns:**
java.util.Collection<com.groupdocs.parser.data.PageTableAreaCell> - Una colección de celdas de tabla

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Obtiene el número total de filas de la tabla.


**Returns:**
int - Un valor entero que contiene el número total de filas de la tabla.

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Obtiene el número total de columnas de la tabla.


**Returns:**
int - Un valor entero que contiene el número total de columnas de la tabla.

### getRowHeight(int rowIndex) {#getRowHeight-int-}
```
public double getRowHeight(int rowIndex)
```


Devuelve la altura de la fila.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rowIndex | int | El índice basado en cero de la fila. |
|

**Returns:**
double - Un valor double que representa la altura de la fila.

### getColumnWidth(int columnIndex) {#getColumnWidth-int-}
```
public double getColumnWidth(int columnIndex)
```


Devuelve el ancho de la columna.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | columnIndex | int | El índice basado en cero de la columna. |
|

**Returns:**
double - Un valor double que representa el ancho de la columna.

### getCell(int rowIndex, int columnIndex) {#getCell-int-int-}
```
public PageTableAreaCell getCell(int rowIndex, int columnIndex)
```


Obtiene la celda de la tabla por índices de fila y columna.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rowIndex | int | El índice basado en cero de la fila de la celda. |
|
|  | columnIndex | int | El índice basado en cero de la columna de la celda. |
|

**Returns:**
[PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) - An instance of [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) class;  null  if no cell is found.


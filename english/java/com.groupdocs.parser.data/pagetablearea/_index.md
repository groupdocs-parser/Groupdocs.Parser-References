---
title: PageTableArea
second_title: GroupDocs.Parser for Java API Reference
description: Represents a table page area which is used to represent a table in the parsing by template functionality.
type: docs
weight: 22
url: /java/com.groupdocs.parser.data/pagetablearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTableArea extends PageArea
```

Represents a table page area which is used to represent a table in the parsing by template functionality.

[PageTableArea](../../com.groupdocs.parser.data/pagetablearea) class is used to organize inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class in table structure.
## Constructors

| Constructor | Description |
| --- | --- |
| [PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)](#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initializes a new instance of the [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) class. |
## Methods

| Method | Description |
| --- | --- |
| [getRowCount()](#getRowCount--) | Gets the total number of the table rows. |
| [getColumnCount()](#getColumnCount--) | Gets the total number of the table colums. |
| [getRowHeight(int rowIndex)](#getRowHeight-int-) | Returns the row height. |
| [getColumnWidth(int columnIndex)](#getColumnWidth-int-) | Returns the column width. |
| [getCell(int rowIndex, int columnIndex)](#getCell-int-int-) | Gets the table cell by row and column indexes. |
### PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle) {#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)
```


Initializes a new instance of the [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rows | java.lang.Iterable<java.lang.Double> | The collection of row heights. |
| columns | java.lang.Iterable<java.lang.Double> | The collection of column widths. |
| cells | java.lang.Iterable<com.groupdocs.parser.data.PageTableAreaCell> | The collection of cells. |
| page | [Page](../../com.groupdocs.parser.data/page) | The page that contains the table. |
| rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | The rectangular area that contains the table. |

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Gets the total number of the table rows.

**Returns:**
int - An integer value that contains the total number of the table rows.
### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Gets the total number of the table colums.

**Returns:**
int - An integer value that contains the total number of the table columns.
### getRowHeight(int rowIndex) {#getRowHeight-int-}
```
public double getRowHeight(int rowIndex)
```


Returns the row height.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | The zero-based index of the row. |

**Returns:**
double - A double value that represents the height of the row.
### getColumnWidth(int columnIndex) {#getColumnWidth-int-}
```
public double getColumnWidth(int columnIndex)
```


Returns the column width.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | The zero-based index of the column. |

**Returns:**
double - A double value that represents the width of the column.
### getCell(int rowIndex, int columnIndex) {#getCell-int-int-}
```
public PageTableAreaCell getCell(int rowIndex, int columnIndex)
```


Gets the table cell by row and column indexes.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | The zero-based index of the cell row. |
| columnIndex | int | The zero-based index of the cell column. |

**Returns:**
[PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) - An instance of [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) class;  null  if no cell is found.

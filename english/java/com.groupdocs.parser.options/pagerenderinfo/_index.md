---
title: PageRenderInfo
second_title: GroupDocs.Parser for Java API Reference
description: Represents the information of how a page is rendered.
type: docs
weight: 30
url: /java/com.groupdocs.parser.options/pagerenderinfo/
---
**Inheritance:**
java.lang.Object
```
public class PageRenderInfo
```

Represents the information of how a page is rendered.

Some documents (spreadsheets, for example) are not possible to render a page as a single image. For those documents a page is rendered as a set of tiles. These tiles are placed in the rectangular table.

 RowCount  and  ColumnCount  represent the total number of rows and columns of this table. If document page is rendered to the single image these properties are equal to 1.
## Constructors

| Constructor | Description |
| --- | --- |
| [PageRenderInfo(int pageNumber, int rowCount, int columnCount)](#PageRenderInfo-int-int-int-) | Initializes a new instance of the [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo) class. |
## Methods

| Method | Description |
| --- | --- |
| [getPageNumber()](#getPageNumber--) | Gets the page number. |
| [getRowCount()](#getRowCount--) | Get the total number of tiles rows. |
| [getColumnCount()](#getColumnCount--) | Get the total number of tiles columns. |
| [getColumn(int tileIndex)](#getColumn-int-) | Returns the index of column where the tile with  tileIndex  is placed. |
| [getRow(int tileIndex)](#getRow-int-) | Returns the index of row where the tile with  tileIndex  is placed. |
### PageRenderInfo(int pageNumber, int rowCount, int columnCount) {#PageRenderInfo-int-int-int-}
```
public PageRenderInfo(int pageNumber, int rowCount, int columnCount)
```


Initializes a new instance of the [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageNumber | int | The number of the page (starts with 1). |
| rowCount | int | The total number of tiles rows. |
| columnCount | int | The total number of tiles columns. |

### getPageNumber() {#getPageNumber--}
```
public int getPageNumber()
```


Gets the page number.

**Returns:**
int - The integer value that represents the page number (starts with 1).
### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Get the total number of tiles rows.

**Returns:**
int - The integer value that represents the total number of tiles rows.
### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Get the total number of tiles columns.

**Returns:**
int - The integer value that represents the total number of tiles columns.
### getColumn(int tileIndex) {#getColumn-int-}
```
public int getColumn(int tileIndex)
```


Returns the index of column where the tile with  tileIndex  is placed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tileIndex | int | The zero-based index of the tile. |

**Returns:**
int - The zero-based integer value that represents the column index.
### getRow(int tileIndex) {#getRow-int-}
```
public int getRow(int tileIndex)
```


Returns the index of row where the tile with  tileIndex  is placed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tileIndex | int | The zero-based index of the tile. |

**Returns:**
int - The zero-based integer value that represents the row index.

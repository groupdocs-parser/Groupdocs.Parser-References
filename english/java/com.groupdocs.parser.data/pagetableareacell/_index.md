---
title: PageTableAreaCell
second_title: GroupDocs.Parser for Java API Reference
description: Represents a table cell which is used in  class.
type: docs
weight: 22
url: /java/com.groupdocs.parser.data/pagetableareacell/
---
**Inheritance:**
java.lang.Object
```
public class PageTableAreaCell
```

Represents a table cell which is used in [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) class.
## Constructors

| Constructor | Description |
| --- | --- |
| [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-) | Initializes a new instance of the [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) class. |
| [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-) | Initializes a new instance of the [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) class. |
## Methods

| Method | Description |
| --- | --- |
| [getRowIndex()](#getRowIndex--) | Gets the row index. |
| [getColumnIndex()](#getColumnIndex--) | Gets the column index. |
| [getRowSpan()](#getRowSpan--) | Gets the total number of rows that contain the table cell. |
| [getColumnSpan()](#getColumnSpan--) | Gets the total number of columns that contain the table cell. |
| [getPageArea()](#getPageArea--) | Gets the table cell value. |
| [getText()](#getText--) | Gets the table cell text value. |
### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)
```


Initializes a new instance of the [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | The zero-based index of the row. |
| columnIndex | int | The zero-based index of the column. |
| pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | The value of the table cell. |

### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)
```


Initializes a new instance of the [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | The zero-based index of the row. |
| columnIndex | int | The zero-based index of the column. |
| pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | The value of the table cell. |
| rowSpan | int | The total number of rows that contain the table cell. |
| columnSpan | int | The total number of columns that contain the table cell. |

### getRowIndex() {#getRowIndex--}
```
public int getRowIndex()
```


Gets the row index.

**Returns:**
int - A zero-based index of the first row that contains the table cell.
### getColumnIndex() {#getColumnIndex--}
```
public int getColumnIndex()
```


Gets the column index.

**Returns:**
int - A zero-based index of the first column that contains the table cell.
### getRowSpan() {#getRowSpan--}
```
public int getRowSpan()
```


Gets the total number of rows that contain the table cell.

**Returns:**
int - A positive integer value that represents the total number of rows that contain the table cell.
### getColumnSpan() {#getColumnSpan--}
```
public int getColumnSpan()
```


Gets the total number of columns that contain the table cell.

**Returns:**
int - A positive integer value that represents the total number of columns that contain the table cell.
### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


Gets the table cell value.

**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - Depending on cell [PageArea](../../com.groupdocs.parser.data/pagearea) property can contain any of the inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class.
### getText() {#getText--}
```
public String getText()
```


Gets the table cell text value.

**Returns:**
java.lang.String - A string that represents a text value of the cell;  null  if cell doesn't contain a text value.

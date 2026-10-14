---
title: "PageTableAreaCell"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示在类中使用的表格单元格。"
type: docs
weight: 23
url: /zh/java/com.groupdocs.parser.data/pagetableareacell/
---
**Inheritance:**
java.lang.Object
```
public class PageTableAreaCell
```

表示在 [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) 类中使用的表格单元格。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-) | 初始化 [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) 类的新实例。 |
|
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-) | 初始化 [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getRowIndex()](#getRowIndex--) | 获取行索引。 |
|
|  | [getColumnIndex()](#getColumnIndex--) | 获取列索引。 |
|
|  | [getRowSpan()](#getRowSpan--) | 获取包含该表格单元格的行总数。 |
|
|  | [getColumnSpan()](#getColumnSpan--) | 获取包含该表格单元格的列总数。 |
|
|  | [getPageArea()](#getPageArea--) | 获取表格单元格的值。 |
|
|  | [getText()](#getText--) | 获取表格单元格的文本值。 |
|
### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)
```


初始化 [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rowIndex | int | 行的零基索引。 |
|
|  | columnIndex | int | 列的零基索引。 |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | 表格单元格的值。 |
|

### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)
```


初始化 [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rowIndex | int | 行的零基索引。 |
|
|  | columnIndex | int | 列的零基索引。 |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | 表格单元格的值。 |
|
|  | rowSpan | int | 包含该单元格的行总数。 |
|
|  | columnSpan | int | 包含该单元格的列总数。 |
|

### getRowIndex() {#getRowIndex--}
```
public int getRowIndex()
```


获取行索引。


**Returns:**
int - 包含该单元格的第一行的零基索引。

### getColumnIndex() {#getColumnIndex--}
```
public int getColumnIndex()
```


获取列索引。


**Returns:**
int - 包含该单元格的第一列的零基索引。

### getRowSpan() {#getRowSpan--}
```
public int getRowSpan()
```


获取包含该表格单元格的行总数。


**Returns:**
int - 表示包含该单元格的行总数的正整数值。

### getColumnSpan() {#getColumnSpan--}
```
public int getColumnSpan()
```


获取包含该表格单元格的列总数。


**Returns:**
int - 表示包含该单元格的列总数的正整数值。

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


获取表格单元格的值。


**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - Depending on cell [PageArea](../../com.groupdocs.parser.data/pagearea) property can contain any of the inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class.

### getText() {#getText--}
```
public String getText()
```


获取表格单元格的文本值。


**Returns:**
java.lang.String - 表示单元格文本值的字符串；如果单元格不包含文本值，则为 null。


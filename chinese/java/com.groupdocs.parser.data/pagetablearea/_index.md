---
title: "PageTableArea"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示用于在基于模板的解析功能中表示表格的页面表格区域。"
type: docs
weight: 22
url: /zh/java/com.groupdocs.parser.data/pagetablearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTableArea extends PageArea
```

表示用于在基于模板的解析功能中表示表格的页面表格区域。

[PageTableArea](../../com.groupdocs.parser.data/pagetablearea) class is used to organize inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class in table structure.

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)](#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | 初始化一个新的 [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) 类实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getCells()](#getCells--) | 获取单元格集合。 |
|
|  | [getRowCount()](#getRowCount--) | 获取表格行的总数。 |
|
|  | [getColumnCount()](#getColumnCount--) | 获取表格列的总数。 |
|
|  | [getRowHeight(int rowIndex)](#getRowHeight-int-) | 返回行高。 |
|
|  | [getColumnWidth(int columnIndex)](#getColumnWidth-int-) | 返回列宽。 |
|
|  | [getCell(int rowIndex, int columnIndex)](#getCell-int-int-) | 通过行列索引获取表格单元格。 |
|
### PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle) {#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)
```


初始化一个新的 [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) 类实例。

注意：C# 项目将此构造函数标记为
internal
(commit 954951f)。在 Java 中，"internal-to-the-assembly"
无法干净地翻译为 package-private，因为生产者（
WordProcessingParser
,
TableAreaParser
,
等）位于
com.groupdocs.parser
, 而不是
com.groupdocs.parser.data
。因此构造函数保持

public
以便跨包构造仍然有效。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 行 | java.lang.Iterable<java.lang.Double> | 行高的集合。 |
|
|  | 列 | java.lang.Iterable<java.lang.Double> | 列宽的集合。 |
|
|  | 单元格 | java.lang.Iterable<com.groupdocs.parser.data.PageTableAreaCell> | 单元格的集合。 |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | 包含该表格的页面。 |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 包含表格的矩形区域。 |
|

### getCells() {#getCells--}
```
public Collection<PageTableAreaCell> getCells()
```


获取单元格的集合。一个纯只读的表格单元格集合。


**Returns:**
java.util.Collection<com.groupdocs.parser.data.PageTableAreaCell> - 表格单元格的集合

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


获取表格行的总数。


**Returns:**
int - 包含表格行总数的整数值。

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


获取表格列的总数。


**Returns:**
int - 包含表格列总数的整数值。

### getRowHeight(int rowIndex) {#getRowHeight-int-}
```
public double getRowHeight(int rowIndex)
```


返回行高。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rowIndex | int | 行的零基索引。 |
|

**Returns:**
double - 表示行高的双精度值。

### getColumnWidth(int columnIndex) {#getColumnWidth-int-}
```
public double getColumnWidth(int columnIndex)
```


返回列宽。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | columnIndex | int | 列的零基索引。 |
|

**Returns:**
double - 表示列宽的双精度值。

### getCell(int rowIndex, int columnIndex) {#getCell-int-int-}
```
public PageTableAreaCell getCell(int rowIndex, int columnIndex)
```


通过行列索引获取表格单元格。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rowIndex | int | 单元格行的零基索引。 |
|
|  | columnIndex | int | 单元格列的零基索引。 |
|

**Returns:**
[PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) - An instance of [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) class;  null  if no cell is found.


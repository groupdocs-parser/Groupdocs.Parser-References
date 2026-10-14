---
title: "PageRenderInfo"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示页面渲染方式的信息。"
type: docs
weight: 30
url: /zh/java/com.groupdocs.parser.options/pagerenderinfo/
---
**Inheritance:**
java.lang.Object
```
public class PageRenderInfo
```

表示页面渲染方式的信息。

某些文档（例如电子表格）无法将页面渲染为
单个图像。对于这些文档，页面会被渲染为一组瓦片。
这些瓦片被放置在矩形表格中。


RowCount
和
ColumnCount
表示行数和列数的总数
此表格的。如果文档页面被渲染为单个图像，这些属性的值为 1。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [PageRenderInfo(int pageNumber, int rowCount, int columnCount)](#PageRenderInfo-int-int-int-) | 初始化 [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | 获取页码。 |
|
|  | [getRowCount()](#getRowCount--) | 获取瓦片行的总数。 |
|
|  | [getColumnCount()](#getColumnCount--) | 获取瓦片列的总数。 |
|
|  | [getColumn(int tileIndex)](#getColumn-int-) | 返回放置 tileIndex 瓦片的列索引。 |
|
|  | [getRow(int tileIndex)](#getRow-int-) | 返回放置 tileIndex 瓦片的行索引。 |
|
### PageRenderInfo(int pageNumber, int rowCount, int columnCount) {#PageRenderInfo-int-int-int-}
```
public PageRenderInfo(int pageNumber, int rowCount, int columnCount)
```


初始化 [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pageNumber | int | 页面的编号（从 1 开始）。 |
|
|  | rowCount | int | 瓦片行的总数。 |
|
|  | columnCount | int | 瓦片列的总数。 |
|

### getPageNumber() {#getPageNumber--}
```
public int getPageNumber()
```


获取页码。


**Returns:**
int - 表示页面编号的整数值（从 1 开始）。

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


获取瓦片行的总数。


**Returns:**
int - 表示瓦片行总数的整数值。

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


获取瓦片列的总数。


**Returns:**
int - 表示瓦片列总数的整数值。

### getColumn(int tileIndex) {#getColumn-int-}
```
public int getColumn(int tileIndex)
```


返回放置 tileIndex 瓦片的列索引。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | tileIndex | int | 瓦片的零基索引。 |
|

**Returns:**
int - 表示列索引的零基整数值。

### getRow(int tileIndex) {#getRow-int-}
```
public int getRow(int tileIndex)
```


返回放置 tileIndex 瓦片的行索引。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | tileIndex | int | 瓦片的零基索引。 |
|

**Returns:**
int - 表示行索引的零基整数值。


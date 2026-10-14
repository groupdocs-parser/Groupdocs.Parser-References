---
title: "PageInfo"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示文档页面信息。"
type: docs
weight: 29
url: /zh/java/com.groupdocs.parser.options/pageinfo/
---
**Inheritance:**
java.lang.Object
```
public class PageInfo
```

表示文档页面信息。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [PageInfo(int pageNumber, int width, int height)](#PageInfo-int-int-int-) | 初始化 [PageInfo](../../com.groupdocs.parser.options/pageinfo) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | 获取页码。 |
|
|  | [getWidth()](#getWidth--) | 获取页面宽度。 |
|
|  | [getHeight()](#getHeight--) | 获取页面高度。 |
|
### PageInfo(int pageNumber, int width, int height) {#PageInfo-int-int-int-}
```
public PageInfo(int pageNumber, int width, int height)
```


初始化 [PageInfo](../../com.groupdocs.parser.options/pageinfo) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pageNumber | int | 页面编号。 |
|
|  | 宽度 | int | 页面宽度。 |
|
|  | 高度 | int | 页面高度。 |
|

### getPageNumber() {#getPageNumber--}
```
public int getPageNumber()
```


获取页码。


**Returns:**
int - 一个基于零的整数值，表示页面编号。

### getWidth() {#getWidth--}
```
public int getWidth()
```


获取页面宽度。


**Returns:**
int - 一个表示页面宽度的整数值。

### getHeight() {#getHeight--}
```
public int getHeight()
```


获取页面高度。


**Returns:**
int - 一个表示页面高度的整数值。


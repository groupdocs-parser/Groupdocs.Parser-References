---
title: "页面"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示文档页信息，例如页索引和页大小。"
type: docs
weight: 16
url: /zh/java/com.groupdocs.parser.data/page/
---
**Inheritance:**
java.lang.Object
```
public class Page
```

表示文档页面信息，例如页面索引和页面大小。它用于表示在模板解析功能中包含 [PageArea](../../com.groupdocs.parser.data/pagearea) 类的继承者的页面。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [Page(int index, Size size)](#Page-int-com.groupdocs.parser.data.Size-) | 初始化 [Page](../../com.groupdocs.parser.data/page) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getIndex()](#getIndex--) | 获取页面索引。 |
|
|  | [getSize()](#getSize--) | 获取页面大小。 |
|
### Page(int index, Size size) {#Page-int-com.groupdocs.parser.data.Size-}
```
public Page(int index, Size size)
```


初始化 [Page](../../com.groupdocs.parser.data/page) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 索引 | int | 页面索引。 |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | 页面大小。 |
|

### getIndex() {#getIndex--}
```
public int getIndex()
```


获取页面索引。


**Returns:**
int - 页面从零开始的索引。

### getSize() {#getSize--}
```
public Size getSize()
```


获取页面大小。


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the page.


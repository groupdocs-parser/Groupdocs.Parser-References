---
title: "文档页面数据"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示文档页的数据。"
type: docs
weight: 12
url: /zh/java/com.groupdocs.parser.data/documentpagedata/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.DocumentData](../../com.groupdocs.parser.data/documentdata)
```
public class DocumentPageData extends DocumentData
```

表示文档页面的数据。它由包含文档页面字段数据的 [FieldData](../../com.groupdocs.parser.data/fielddata) 对象组成。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [DocumentPageData(Iterable<FieldData> fields, int pageIndex)](#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-) | 初始化 [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getPageIndex()](#getPageIndex--) | 获取页面索引。 |
|
### DocumentPageData(Iterable<FieldData> fields, int pageIndex) {#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-}
```
public DocumentPageData(Iterable<FieldData> fields, int pageIndex)
```


初始化 [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 字段 | java.lang.Iterable<com.groupdocs.parser.data.FieldData> | 字段数据的集合。 |
|
|  | pageIndex | int | 从零开始的页面索引。 |
|

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


获取页面索引。


**Returns:**
int - 页面从零开始的索引。


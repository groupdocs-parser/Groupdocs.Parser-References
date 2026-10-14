---
title: "页面组区域"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示用于在基于模板的解析功能中对文档页不同类型块进行分组的页面区域组。"
type: docs
weight: 19
url: /zh/java/com.groupdocs.parser.data/pagegrouparea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageGroupArea extends PageArea
```

表示用于在基于模板的解析功能中对文档页不同类型块进行分组的页面区域组。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [PageGroupArea(Iterable<PageArea> areas, Page page)](#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-) | 初始化 [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getAreas()](#getAreas--) | 获取分组页面区域的集合。 |
|
### PageGroupArea(Iterable<PageArea> areas, Page page) {#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-}
```
public PageGroupArea(Iterable<PageArea> areas, Page page)
```


初始化 [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | areas | java.lang.Iterable<com.groupdocs.parser.data.PageArea> | 待分组的页面区域集合。 |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | 包含该区域的页面。 |
|

### getAreas() {#getAreas--}
```
public Iterable<PageArea> getAreas()
```


获取分组页面区域的集合。


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageArea> - [PageArea](../../com.groupdocs.parser.data/pagearea) 对象的集合。


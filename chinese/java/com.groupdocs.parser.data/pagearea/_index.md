---
title: "页面区域"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示用于在基于模板的解析功能中表示文档页块的页面区域抽象基类。"
type: docs
weight: 17
url: /zh/java/com.groupdocs.parser.data/pagearea/
---
**Inheritance:**
java.lang.Object
```
public abstract class PageArea
```

表示用于在基于模板的解析功能中表示文档页块的页面区域抽象基类。

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | 获取矩形区域。 |
|
|  | [getPage()](#getPage--) | 获取文档页面信息，例如页面索引和页面大小。 |
|
### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


获取矩形区域。


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area of the page that contains the page area.

### getPage() {#getPage--}
```
public Page getPage()
```


获取文档页面信息，例如页面索引和页面大小。


**Returns:**
[Page](../../com.groupdocs.parser.data/page) - An instance of [Page](../../com.groupdocs.parser.data/page) class that represents the page that contains the page area.


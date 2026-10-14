---
title: "PageHyperlinkArea"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示用于在页面上表示超链接的页面区域。"
type: docs
weight: 20
url: /zh/java/com.groupdocs.parser.data/pagehyperlinkarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageHyperlinkArea extends PageArea
```

表示用于在页面上表示超链接的页面区域。

以下方法的返回值使用 [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) 类的实例：

* [Parser.getHyperlinks()](../../com.groupdocs.parser/parser#getHyperlinks--)
* [Parser.getHyperlinks(PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-PageAreaOptions-)
* [Parser.getHyperlinks(int)](../../com.groupdocs.parser/parser#getHyperlinks-int-)
* [Parser.getHyperlinks(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-int--PageAreaOptions-)

请参阅那里的使用示例。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)](#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | 初始化 [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getText()](#getText--) | 获取超链接文本。 |
|
|  | [getUrl()](#getUrl--) | 获取超链接 URL。 |
|
### PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle) {#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)
```


初始化 [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文本 | java.lang.String | 超链接文本。 |
|
|  | url | java.lang.String | 超链接 URL。 |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | 包含超链接的页面。 |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 包含超链接的矩形区域。 |
|

### getText() {#getText--}
```
public String getText()
```


获取超链接文本。


**Returns:**
java.lang.String - 表示超链接文本的字符串值。

### getUrl() {#getUrl--}
```
public String getUrl()
```


获取超链接 URL。


**Returns:**
java.lang.String - 表示超链接 URL 的字符串值。


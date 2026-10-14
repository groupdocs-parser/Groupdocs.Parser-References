---
title: "PageTextArea"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示用于在基于模板或表单解析功能中表示文本值的页面文本区域。"
type: docs
weight: 24
url: /zh/java/com.groupdocs.parser.data/pagetextarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTextArea extends PageArea
```

表示用于在基于模板或表单解析功能中表示文本值的页面文本区域。

以下方法的返回值使用 [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 类的实例：

* [Parser.getTextAreas()](../../com.groupdocs.parser/parser#getTextAreas--)
* [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-)
* [Parser.getTextAreas(int)](../../com.groupdocs.parser/parser#getTextAreas-int-)
* [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-)

同样， [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 类的实例用作 [PageArea](../../com.groupdocs.parser.data/pagearea) 属性的值。
\*

请参阅那里的使用示例。

文本区域可以是单一的或复合的。在第一种情况下，它包含一个被矩形区域限定的文本。
在第二种情况下，它包含其他文本区域；文本和表格属性由子文本区域计算。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [PageTextArea(String text, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | 初始化 [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 类的新实例。 |
|
|  | [PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | 初始化 [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 类的新实例。 |
|
|  | [PageTextArea(Iterable<PageTextArea> areas, Page page)](#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-) | 初始化 [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getText()](#getText--) | 获取文本。 |
|
|  | [getBaseLine()](#getBaseLine--) | 获取基线。 |
|
|  | [getTextStyle()](#getTextStyle--) | 获取文本样式，例如字体大小、字体名称等。 |
|
|  | [getAreas()](#getAreas--) | 获取子文本页面区域的集合。 |
|
### PageTextArea(String text, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Page page, Rectangle rectangle)
```


初始化 [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文本 | java.lang.String | 文本的值。 |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | 包含文本区域的页面。 |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 包含文本区域的矩形区域。 |
|

### PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)
```


初始化 [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文本 | java.lang.String | 文本的值。 |
|
|  | baseLine | java.lang.Double | 文本的基线。 |
|
|  | textStyle | [TextStyle](../../com.groupdocs.parser.data/textstyle) | 文本的样式。 |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | 包含文本区域的页面。 |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 包含文本区域的矩形区域。 |
|

### PageTextArea(Iterable<PageTextArea> areas, Page page) {#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-}
```
public PageTextArea(Iterable<PageTextArea> areas, Page page)
```


初始化 [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | areas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | 子文本页面区域的集合。 |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | 包含文本区域的页面。 |
|

### getText() {#getText--}
```
public String getText()
```


获取文本。


**Returns:**
java.lang.String - 表示文本页面区域值的字符串。

### getBaseLine() {#getBaseLine--}
```
public double getBaseLine()
```


获取基线。


**Returns:**
double - 表示基线的 double 值。

### getTextStyle() {#getTextStyle--}
```
public TextStyle getTextStyle()
```


获取文本样式，例如字体大小、字体名称等。


**Returns:**
[TextStyle](../../com.groupdocs.parser.data/textstyle) - An instance of [TextStyle](../../com.groupdocs.parser.data/textstyle) class that represents the text style.

### getAreas() {#getAreas--}
```
public List<PageTextArea> getAreas()
```


获取子文本页面区域的集合。


**Returns:**
java.util.List<com.groupdocs.parser.data.PageTextArea> - 子文本页面区域的集合；如果文本页面区域没有子项则为空。


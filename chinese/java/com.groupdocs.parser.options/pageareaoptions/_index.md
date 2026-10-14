---
title: "PageAreaOptions"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供用于页面区域提取的选项。"
type: docs
weight: 28
url: /zh/java/com.groupdocs.parser.options/pageareaoptions/
---
**Inheritance:**
java.lang.Object
```
public class PageAreaOptions
```

提供用于页面区域提取的选项。

在 [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-) 中使用 [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) 类的实例作为参数。
以及 [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-) 方法。请参阅那里的使用示例。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [PageAreaOptions(Rectangle rectangle)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-) | 使用被忽略边框的大小初始化 [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) 类的新实例。 |
|
|  | [PageAreaOptions(Rectangle rectangle, double rectangleTolerance)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-) | 初始化 [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | 获取包含页面区域的矩形区域。 |
|
|  | [getRectangleTolerance()](#getRectangleTolerance--) | 获取在矩形区域捕获时被忽略的边框大小。 |
|
### PageAreaOptions(Rectangle rectangle) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageAreaOptions(Rectangle rectangle)
```


使用被忽略边框的大小初始化 [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 包含页面区域的矩形区域。 |
|

### PageAreaOptions(Rectangle rectangle, double rectangleTolerance) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-}
```
public PageAreaOptions(Rectangle rectangle, double rectangleTolerance)
```


初始化 [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 包含页面区域的矩形区域。 |
|
|  | rectangleTolerance | double | 在矩形区域捕获时被忽略的边框大小。它以文本项高度的比例来衡量。 |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


获取包含页面区域的矩形区域。


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


获取在矩形区域捕获时被忽略的边框大小。它以文本项高度的比例来衡量。


**Returns:**
double - 从 0（无边框）到 1（忽略整个元素）的 double 值。


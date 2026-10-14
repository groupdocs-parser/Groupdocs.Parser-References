---
title: "PageTableAreaOptions"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供用于页面表格区域提取的选项。"
type: docs
weight: 31
url: /zh/java/com.groupdocs.parser.options/pagetableareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTableAreaOptions extends PageAreaOptions
```

提供用于页面表格区域提取的选项。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [PageTableAreaOptions(TemplateTableLayout tableLayout)](#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-) | 初始化 [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) 类的新实例。 |
|
|  | [PageTableAreaOptions(Rectangle rectangle)](#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-) | 使用搜索矩形且无固定布局，初始化 [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getTableLayout()](#getTableLayout--) | 获取定义页面上表格的表布局。 |
|
### PageTableAreaOptions(TemplateTableLayout tableLayout) {#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-}
```
public PageTableAreaOptions(TemplateTableLayout tableLayout)
```


初始化 [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | tableLayout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | 定义页面上表格的表布局。 |
|

### PageTableAreaOptions(Rectangle rectangle) {#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageTableAreaOptions(Rectangle rectangle)
```


使用搜索矩形且无固定布局，初始化 [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) 类的新实例。

用于将自动检测的表格限制在页面的特定区域。对应 C# 实现。

new PageTableAreaOptions(null) { Rectangle = ... }
模式。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 页面上应检测表格的矩形区域；传入 null 以搜索整个页面。 |
|

### getTableLayout() {#getTableLayout--}
```
public TemplateTableLayout getTableLayout()
```


获取定义页面上表格的表布局。


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instane of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class.


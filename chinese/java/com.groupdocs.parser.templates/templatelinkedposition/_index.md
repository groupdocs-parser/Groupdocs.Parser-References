---
title: "TemplateLinkedPosition"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供使用链接字段的模板字段位置。"
type: docs
weight: 15
url: /zh/java/com.groupdocs.parser.templates/templatelinkedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateLinkedPosition extends TemplatePosition
```

提供使用链接字段的模板字段位置。

以下示例展示了在已知发票号码字段的情况下的代码
位于 \"Invoice number\" 字符串的右侧时使用以下代码：

````
// Create a regex template field to find "Invoice Number" text
 TemplateField invoice = new TemplateField(new TemplateRegexPosition("Invoice Number"), "Invoice");

 // Create a related template field associated with "Invoice" field and extract the value on the right of it
 TemplateField invoiceNumber = new TemplateField(
     new TemplateLinkedPosition("invoice", new Size(100, 15), new TemplateLinkedPositionEdges(false, false, true, false)),
     "InvoiceNumber");
 
````


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-) | 初始化一个新的 [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) 类的实例。 |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-) | 初始化一个新的 [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) 类的实例，使用大写名称。 |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-) | 初始化一个新的 [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) 类的实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getLinkedFieldName()](#getLinkedFieldName--) | 获取链接字段的名称。 |
|
|  | [getSearchArea()](#getSearchArea--) | 获取搜索字段的区域大小。 |
|
|  | [isAutoScale()](#isAutoScale--) | 获取指示 SearchArea 是否按链接字段大小缩放的值。 |
|
|  | [getEdges()](#getEdges--) | 获取搜索字段时链接字段的边缘。 |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)
```


初始化一个新的 [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) 类的实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | 链接字段的名称。 |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | 搜索字段的区域大小。 |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | 搜索字段时链接字段的边缘。 |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)
```


初始化一个新的 [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) 类的实例，使用大写名称。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | 链接字段的名称。 |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | 搜索字段的区域大小。 |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | 搜索字段时链接字段的边缘。 |
|
|  | autoScale | boolean | 指示 searchArea 是否按链接字段大小缩放的值。 |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)
```


初始化一个新的 [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) 类的实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | 链接字段的名称。 |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | 搜索字段的区域大小。 |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | 搜索字段时链接字段的边缘。 |
|
|  | autoScale | boolean | 指示 searchArea 是否按链接字段大小缩放的值。\\ |
|
|  | useUpperCaseName | boolean | 指示是否将  名称  转换为大写的值。 |
|

### getLinkedFieldName() {#getLinkedFieldName--}
```
public String getLinkedFieldName()
```


获取链接字段的名称。


**Returns:**
java.lang.String - 表示链接字段名称的大写字符串值。

### getSearchArea() {#getSearchArea--}
```
public Size getSearchArea()
```


获取搜索字段的区域大小。


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the area where a field is searched.

### isAutoScale() {#isAutoScale--}
```
public Boolean isAutoScale()
```


获取指示 SearchArea 是否按链接字段大小缩放的值。


**Returns:**
java.lang.Boolean - 如果 SearchArea 按链接字段大小缩放，则为 {code true}；否则为 false。

### getEdges() {#getEdges--}
```
public TemplateLinkedPositionEdges getEdges()
```


获取搜索字段时链接字段的边缘。


**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that represents the edges of the linked field where a field is searched.

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


创建当前位置的副本，所有坐标按给定因子缩放。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 因子 | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)

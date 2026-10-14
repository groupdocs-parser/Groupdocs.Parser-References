---
title: "TemplateLinkedPositionEdges"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供链接字段的边缘，以搜索文本字段。"
type: docs
weight: 16
url: /zh/java/com.groupdocs.parser.templates/templatelinkedpositionedges/
---
**Inheritance:**
java.lang.Object
```
public class TemplateLinkedPositionEdges
```

提供链接字段的边缘，其中搜索文本字段。 [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) 在 [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) 类中使用。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)](#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-) | 初始化 [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [isEmpty()](#isEmpty--) | 获取指示实例是否为空的值。 |
|
|  | [isLeft()](#isLeft--) | 获取指示是否从链接字段的左侧搜索字段的值。 |
|
|  | [isTop()](#isTop--) | 获取指示是否从链接字段的顶部搜索字段的值。 |
|
|  | [isRight()](#isRight--) | 获取指示是否从链接字段的右侧搜索字段的值。 |
|
|  | [isBottom()](#isBottom--) | 获取指示是否从链接字段的底部搜索字段的值。 |
|
|  | [parse(String s)](#parse-java.lang.String-) | 将边缘的字符串表示转换为其对应的类。 |
|
| [toString()](#toString--) |  |
### TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom) {#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-}
```
public TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)
```


初始化 [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 左 | boolean | 指示是否从链接字段的左侧搜索字段的值。 |
|
|  | 上 | boolean | 指示是否从链接字段的顶部搜索字段的值。 |
|
|  | 右 | boolean | 指示是否从链接字段的右侧搜索字段的值。 |
|
|  | 底部 | boolean | 指示是否从链接字段的底部搜索字段的值。 |
|

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


获取指示实例是否为空的值。


**Returns:**
布尔型 - 如果实例为空（所有字段均为 false），则为 true；否则为 false。

### isLeft() {#isLeft--}
```
public boolean isLeft()
```


获取指示是否从链接字段的左侧搜索字段的值。


**Returns:**
布尔型 - 如果字段从链接字段的左侧搜索，则为 true；否则为 false。

### isTop() {#isTop--}
```
public boolean isTop()
```


获取指示是否从链接字段的顶部搜索字段的值。


**Returns:**
布尔型 - 如果字段从链接字段的顶部搜索，则为 true；否则为 false。

### isRight() {#isRight--}
```
public boolean isRight()
```


获取指示是否从链接字段的右侧搜索字段的值。


**Returns:**
布尔型 - 如果字段从链接字段的右侧搜索，则为 true；否则为 false。

### isBottom() {#isBottom--}
```
public boolean isBottom()
```


获取指示是否从链接字段的底部搜索字段的值。


**Returns:**
布尔型 - 如果字段从链接字段的底部搜索，则为 true；否则为 false。

### parse(String s) {#parse-java.lang.String-}
```
public static TemplateLinkedPositionEdges parse(String s)
```


将边缘的字符串表示转换为其对应的类。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | s | java.lang.String | 包含要转换的边缘的字符串。 |
|

**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String

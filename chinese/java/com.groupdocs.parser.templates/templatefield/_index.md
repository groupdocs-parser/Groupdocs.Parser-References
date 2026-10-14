---
title: "TemplateField"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供模板文本字段。"
type: docs
weight: 12
url: /zh/java/com.groupdocs.parser.templates/templatefield/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateField extends TemplateItem
```

提供模板文本字段。

文本字段是根据其在页面上的位置定义的。定义文本字段有三种方式：

* Using the rectangular area: [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition)
* Using the regular expression: [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition)
* Using the linked field: [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [TemplateField(TemplatePosition position, String name)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-) | 初始化一个新的 [TemplateField](../../com.groupdocs.parser.templates/templatefield) 类实例。 |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-) | 使用大写名称初始化一个新的 [TemplateField](../../com.groupdocs.parser.templates/templatefield) 类实例。 |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-) | 使用大写名称初始化一个新的 [TemplateField](../../com.groupdocs.parser.templates/templatefield) 类实例。 |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-) | 初始化一个新的 [TemplateField](../../com.groupdocs.parser.templates/templatefield) 类实例。 |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | 初始化一个新的 [TemplateField](../../com.groupdocs.parser.templates/templatefield) 类实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getPosition()](#getPosition--) | 获取描述如何在文档页面上查找模板字段的值。 |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateField(TemplatePosition position, String name) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-}
```
public TemplateField(TemplatePosition position, String name)
```


初始化一个新的 [TemplateField](../../com.groupdocs.parser.templates/templatefield) 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | 字段位置。 |
|
|  | 名称 | java.lang.String | 字段名称。 |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex)
```


使用大写名称初始化一个新的 [TemplateField](../../com.groupdocs.parser.templates/templatefield) 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | 字段位置。 |
|
|  | 名称 | java.lang.String | 字段名称。 |
|
|  | pageIndex | java.lang.Integer | 一个整数值，表示模板项所在页面的索引；如果模板项位于任意页面，则为 null。 |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)
```


使用大写名称初始化一个新的 [TemplateField](../../com.groupdocs.parser.templates/templatefield) 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | 字段位置。 |
|
|  | 名称 | java.lang.String | 字段名称。 |
|
|  | pageIndex | java.lang.Integer | 一个整数值，表示模板项所在页面的索引；如果模板项位于任意页面，则为 null。 |
|
|  | pageWidth | java.lang.Double | 用于创建模板项的页面宽度。 |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)
```


初始化一个新的 [TemplateField](../../com.groupdocs.parser.templates/templatefield) 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | 字段位置。 |
|
|  | 名称 | java.lang.String | 字段名称。 |
|
|  | pageIndex | java.lang.Integer | 一个整数值，表示模板项所在页面的索引；如果模板项位于任意页面，则为 null。 |
|
|  | useUpperCaseName | boolean | 指示是否将  名称  转换为大写的值。 |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


初始化一个新的 [TemplateField](../../com.groupdocs.parser.templates/templatefield) 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | 字段位置。 |
|
|  | 名称 | java.lang.String | 字段名称。 |
|
|  | pageIndex | java.lang.Integer | 一个整数值，表示模板项所在页面的索引；如果模板项位于任意页面，则为 null。 |
|
|  | pageWidth | java.lang.Double | 用于创建模板项的页面宽度。 |
|
|  | useUpperCaseName | boolean | 指示是否将  名称  转换为大写的值。 |
|

### getPosition() {#getPosition--}
```
public TemplatePosition getPosition()
```


获取描述如何在文档页面上查找模板字段的值。


**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - An instance of [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) descendant class.

### scale(double factor) {#scale-double-}
```
public TemplateItem scale(double factor)
```


创建当前项的副本，所有坐标均按给定因子缩放。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 因子 | double |  |

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem)

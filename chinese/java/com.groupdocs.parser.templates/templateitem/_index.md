---
title: "TemplateItem"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供模板项的基抽象类。"
type: docs
weight: 14
url: /zh/java/com.groupdocs.parser.templates/templateitem/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplateItem
```

提供模板项的基抽象类。

在 [Template](../../com.groupdocs.parser.templates/template) 集合中使用 [TemplateItem](../../com.groupdocs.parser.templates/templateitem) 类的继承者。

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | 创建当前项的副本，所有坐标均按给定因子缩放。 |
|
|  | [getName()](#getName--) | 获取模板项的名称。 |
|
|  | [getPageIndex()](#getPageIndex--) | 获取模板项的页索引。 |
|
|  | [getPageWidth()](#getPageWidth--) | 获取用于创建模板项的页面宽度。 |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | 获取一个值，指示是否已将  名称  转换为大写。 |
|
### scale(double factor) {#scale-double-}
```
public abstract TemplateItem scale(double factor)
```


创建当前项的副本，所有坐标均按给定因子缩放。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 因子 | double | 缩放因子。 |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - A new [TemplateItem](../../com.groupdocs.parser.templates/templateitem) with scaled coordinates.

### getName() {#getName--}
```
public String getName()
```


获取模板项的名称。


**Returns:**
java.lang.String - 表示模板项名称的大写字符串值。

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


获取模板项的页索引。


**Returns:**
java.lang.Integer - 表示模板项所在页面索引的整数值；如果模板项位于任意页面，则为  null  。

### getPageWidth() {#getPageWidth--}
```
public Double getPageWidth()
```


获取用于创建模板项的页面宽度。


**Returns:**
java.lang.Double - 页面宽度（像素）；如果未知页面宽度，则为  null  。

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


获取一个值，指示是否已将  名称  转换为大写。


**Returns:**
boolean - 一个布尔值，指示是否已将  名称  转换为大写。


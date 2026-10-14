---
title: "TemplatePosition"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供模板位置的基抽象类。"
type: docs
weight: 18
url: /zh/java/com.groupdocs.parser.templates/templateposition/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplatePosition
```

提供模板位置的基抽象类。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [TemplatePosition()](#TemplatePosition--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | 创建当前位置的副本，所有坐标按给定因子缩放。 |
|
### TemplatePosition() {#TemplatePosition--}
```
public TemplatePosition()
```


### scale(double factor) {#scale-double-}
```
public abstract TemplatePosition scale(double factor)
```


创建当前位置的副本，所有坐标按给定因子缩放。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 因子 | double | 缩放因子。 |
|

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - A new [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) with scaled coordinates.


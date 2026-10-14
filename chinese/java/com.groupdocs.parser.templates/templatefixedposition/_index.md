---
title: "TemplateFixedPosition"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供由矩形区域定义的模板字段位置。"
type: docs
weight: 13
url: /zh/java/com.groupdocs.parser.templates/templatefixedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateFixedPosition extends TemplatePosition
```

提供由矩形区域定义的模板字段位置。

这是定义字段位置的最简方式。它需要在页面上设置一个限定字段的矩形区域
字段值。所有包含（即使部分）在该矩形区域内的文本都将被提取为该值：

````
// Create a fixed template field with "Address" name which is bounded by a rectangle at the position (35, 160) and with the size (110, 20)
 TemplateField templateField = new TemplateField(
     new TemplateFixedPosition(new Rectangle(new Point(35, 160), new Size(110, 20))),
     "Address");
 
````


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [TemplateFixedPosition(Rectangle rectangle)](#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-) | 初始化一个新的 [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) 类的实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | 获取包含模板字段的矩形区域。 |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateFixedPosition(Rectangle rectangle) {#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-}
```
public TemplateFixedPosition(Rectangle rectangle)
```


初始化一个新的 [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) 类的实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 包含模板字段的矩形区域。 |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


获取包含模板字段的矩形区域。


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template field.

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

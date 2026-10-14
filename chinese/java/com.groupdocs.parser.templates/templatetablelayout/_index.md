---
title: "TemplateTableLayout"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供模板表布局，供  类用于定义表位置。"
type: docs
weight: 21
url: /zh/java/com.groupdocs.parser.templates/templatetablelayout/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableLayout
```

提供模板表布局，供 [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 类用于定义表位置。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)](#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--) | 初始化 [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | 获取包含表格的矩形区域。 |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | 获取表格列分隔符。 |
|
|  | [getHorizontalSeparators()](#getHorizontalSeparators--) | 获取表格行分隔符。 |
|
|  | [moveTo(Point point)](#moveTo-com.groupdocs.parser.data.Point-) | 创建一个在该点位置具有相同大小和分隔符的新布局。 |
|
|  | [scale(double factor)](#scale-double-) | 创建此布局的副本，所有坐标按给定因子缩放。 |
|
### TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators) {#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--}
```
public TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)
```


初始化 [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | 表格列分隔符。 |
|
|  | horizontalSeparators | java.lang.Iterable<java.lang.Double> | 表格行分隔符。 |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


获取包含表格的矩形区域。


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


获取表格列分隔符。


**Returns:**
java.util.List<java.lang.Double> - 表示表格列分隔符的 x 坐标的 double 值集合。

### getHorizontalSeparators() {#getHorizontalSeparators--}
```
public List<Double> getHorizontalSeparators()
```


获取表格行分隔符。


**Returns:**
java.util.List<java.lang.Double> - 表示表格行分隔符的 y 坐标的 double 值集合。

### moveTo(Point point) {#moveTo-com.groupdocs.parser.data.Point-}
```
public TemplateTableLayout moveTo(Point point)
```


创建一个在该点位置具有相同大小和分隔符的新布局。

此功能允许移动表格布局。

例如，文档的每一页都有表格（或一组文档的每页都有表格）。
这些表格在位置和内容上不同，但具有相同的列和行。在这种情况下，用户
可以在 (0, 0) 处一次性定义 [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) 对象，然后将其移动到特定表格的位置。

如果表格位置取决于页面的其他对象，用户可以定义 [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) 对象
基于模板文档，然后根据锚点对象移动它。例如，如果这是一个摘要表格
随后是详细表格（可能包含不同数量的行）。在这种情况下，用户可以定义
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object on template document (with the known details table rectangle) and then move
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object according to the difference of details table rectangle of template and real document.


moveTo(Point)
方法返回当前对象的副本。用户可以传入任意坐标
（即使是负数——则布局将向左/上移动）。

````
// Create a table layout
 TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 0.0, 25.0, 150.0, 180.0, 230.0 }),
     java.util.Arrays.asList(new Double[] { 0.0, 15.0, 30.0, 45.0, 60.0, 75.0 }));
 // Print a rectangle
 Rectangle rect = layout.getRectangle();
 // Prints: pos: (0, 0) size: (230, 75)
 System.out.println(String.format("pos: (%d, %d) size: (%d, %d)",
         rect.getLeft(), rect.getTop(),
         rect.getSize().getWidth(), rect.getSize().getHeight()));
 // Move layout to the definite table location
 TemplateTableLayout movedLayout = layout.moveTo(new Point(315, 250));
 // Ensure that the first separators are moved:
 System.out.println(movedLayout.getVerticalSeparators().get(0)); // prints: 315
 System.out.println(movedLayout.getHorizontalSeparators().get(0)); // prints: 250
 Rectangle movedRect = movedLayout.getRectangle();
 // Prints: pos: (315, 250) size: (230, 75)
 System.out.println(String.format("pos: (%d, %d) size: (%d, %d)",
         movedRect.getLeft(), movedRect.getTop(),
         movedRect.getSize().getWidth(), movedRect.getSize().getHeight()));
 // movedLayout object is a copy of layout object, thus we can tune separators without the impact on the original layout:
 movedLayout.getHorizontalSeparators().add(90.0);
 System.out.println(movedLayout.getHorizontalSeparators().size()); // prints: 7
 System.out.println(layout.getHorizontalSeparators().size()); // prints: 6
 
````



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | point | [Point](../../com.groupdocs.parser.data/point) | 新布局的位置。 |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new layout with the same size, separators and position in the point.

### scale(double factor) {#scale-double-}
```
public TemplateTableLayout scale(double factor)
```


创建此布局的副本，所有坐标按给定因子缩放。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 因子 | double | 缩放因子。 |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) with scaled separators.


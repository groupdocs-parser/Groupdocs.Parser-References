---
title: "TemplateTableParameters"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供用于表检测算法的参数。"
type: docs
weight: 22
url: /zh/java/com.groupdocs.parser.templates/templatetableparameters/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableParameters
```

提供用于表检测算法的参数。

有两种算法用于检测表格：

* Allows to detect a table in the rectangular area with set columns. This algorithm is useful for simple tables (without merged columns) and provides more accurate detection.
* Allows to detect a table in any place on the page. This is a more complex algorithm. It can detect tables in any place on the page. Additional parameters help to detect a table more correctly.

在某些情况下，当算法无法检测到表格或检测不够准确时，会使用 [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) 类。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--) | 初始化一个新的 [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) 类实例。 |
|
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-) | 初始化一个新的 [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) 类实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | 获取包含表格的矩形区域。 |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | 获取表格列分隔符。 |
|
|  | [hasMergedCells()](#hasMergedCells--) | 获取指示表格是否具有合并单元格的值。 |
|
|  | [getMinRowCount()](#getMinRowCount--) | 获取表格行的最小数量。 |
|
|  | [getMinColumnCount()](#getMinColumnCount--) | 获取表格列的最小数量。 |
|
|  | [getMinVerticalSpace()](#getMinVerticalSpace--) | 获取表格列之间的最小间距。 |
|
|  | [scale(double factor)](#scale-double-) | 创建这些参数的副本，并将所有坐标按给定因子缩放。 |
|
### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)
```


初始化一个新的 [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 包含表格的矩形区域。 |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | 表格列分隔符。 |
|

### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)
```


初始化一个新的 [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 包含表格的矩形区域。 |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | 表格列分隔符。 |
|
|  | mergedCells | java.lang.Boolean | 指示表格是否具有合并单元格的值。 |
|
|  | minRowCount | java.lang.Integer | 表格行的最小数量。 |
|
|  | minColumnCount | java.lang.Integer | 表格列的最小数量。 |
|
|  | minVerticalSpace | java.lang.Integer | 表格列之间的最小间距。 |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


获取包含表格的矩形区域。


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table;  null  if it isn't set.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


获取表格列分隔符。


**Returns:**
java.util.List<java.lang.Double> - 表示表格列分隔符 x 坐标的 double 值集合；如果未设置则为 null。

### hasMergedCells() {#hasMergedCells--}
```
public Boolean hasMergedCells()
```


获取指示表格是否具有合并单元格的值。


**Returns:**
java.lang.Boolean - 如果表格具有合并单元格则为 true；否则为 false。如果未设置则为 null。

### getMinRowCount() {#getMinRowCount--}
```
public Integer getMinRowCount()
```


获取表格行的最小数量。


**Returns:**
java.lang.Integer - 表示表格行最小数量的整数值；如果未设置则为 null。

### getMinColumnCount() {#getMinColumnCount--}
```
public Integer getMinColumnCount()
```


获取表格列的最小数量。


**Returns:**
java.lang.Integer - 表示表格列最小数量的整数值；如果未设置则为 null。

### getMinVerticalSpace() {#getMinVerticalSpace--}
```
public Integer getMinVerticalSpace()
```


获取表格列之间的最小间距。


**Returns:**
java.lang.Integer - 表示表格列之间最小间距的整数值；如果未设置则为 null。

### scale(double factor) {#scale-double-}
```
public TemplateTableParameters scale(double factor)
```


创建这些参数的副本，并将所有坐标按给定因子缩放。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 因子 | double | 缩放因子。 |
|

**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - A new [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) with scaled coordinates.


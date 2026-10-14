---
title: "TemplateBarcode"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供模板条形码字段。"
type: docs
weight: 11
url: /zh/java/com.groupdocs.parser.templates/templatebarcode/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateBarcode extends TemplateItem
```

提供模板条形码字段。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [TemplateBarcode(Rectangle rectangle, String name)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-) | 初始化一个新的 [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) 类实例。 |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-) | 初始化一个新的 [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) clas，使用 UPPER CASE 名称。 |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-) | 初始化一个新的 [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) 类，使用 UPPER CASE 名称。 |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-) | 初始化一个新的 [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) 类实例。 |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | 初始化一个新的 [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) 类实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | 获取包含模板条形码字段的矩形区域。 |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateBarcode(Rectangle rectangle, String name) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-}
```
public TemplateBarcode(Rectangle rectangle, String name)
```


初始化一个新的 [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 包含模板条形码字段的矩形区域。 |
|
|  | 名称 | java.lang.String | 条形码字段名称。 |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)
```


初始化一个新的 [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) clas，使用 UPPER CASE 名称。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 包含模板条形码字段的矩形区域。 |
|
|  | 名称 | java.lang.String | 条形码字段名称。 |
|
|  | pageIndex | java.lang.Integer | 一个整数值，表示模板项所在页面的索引；如果模板项位于任意页面，则为 null。 |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)
```


初始化一个新的 [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) 类，使用 UPPER CASE 名称。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 包含模板条形码字段的矩形区域。 |
|
|  | 名称 | java.lang.String | 条形码字段名称。 |
|
|  | pageIndex | java.lang.Integer | 一个整数值，表示模板项所在页面的索引；如果模板项位于任意页面，则为 null。 |
|
|  | pageWidth | java.lang.Double | 用于创建模板项的页面宽度。 |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)
```


初始化一个新的 [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 包含模板条形码字段的矩形区域。 |
|
|  | 名称 | java.lang.String | 条形码字段名称。 |
|
|  | pageIndex | java.lang.Integer | 一个整数值，表示模板项所在页面的索引；如果模板项位于任意页面，则为 null。 |
|
|  | useUpperCaseName | boolean | 指示是否将  名称  转换为大写的值。 |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


初始化一个新的 [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 包含模板条形码字段的矩形区域。 |
|
|  | 名称 | java.lang.String | 条形码字段名称。 |
|
|  | pageIndex | java.lang.Integer | 一个整数值，表示模板项所在页面的索引；如果模板项位于任意页面，则为 null。 |
|
|  | pageWidth | java.lang.Double | 用于创建模板项的页面宽度。 |
|
|  | useUpperCaseName | boolean | 指示是否将  名称  转换为大写的值。 |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


获取包含模板条形码字段的矩形区域。


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template barcode field.

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

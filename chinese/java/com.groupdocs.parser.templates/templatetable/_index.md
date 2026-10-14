---
title: "TemplateTable"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供模板表。"
type: docs
weight: 20
url: /zh/java/com.groupdocs.parser.templates/templatetable/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateTable extends TemplateItem
```

提供模板表。

定义表有两种方式：

* Using [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class. In this case the table is defined by its position on the page: rectangular area, columns and rows separators.
* Using [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class. In this case the table is detected automatically by algorithms with set parameters. See [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class for more information.

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-) | 使用大写名称初始化 [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 类的新实例。 |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-) | 使用大写名称初始化 [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 类的新实例。 |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-) | 初始化 [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 类的新实例。 |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | 初始化 [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 类的新实例。 |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-) | 使用大写名称初始化 [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 类的新实例。 |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-) | 初始化 [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 类的新实例。 |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-) | 初始化 [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 类的新实例。 |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | 初始化 [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getLayout()](#getLayout--) | 获取表布局。 |
|
|  | [getParameters()](#getParameters--) | 获取自动模式下检测表的参数。 |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)
```


使用大写名称初始化 [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 类的新实例。

如果无法自动检测表，则通过表布局设置模板表：

````
TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 50.0, 95.0, 275.0 }),
     java.util.Arrays.asList(new Double[] { 325.0, 340.0, 365.0 }));
 TemplateTable table = new TemplateTable(layout, "Details", null);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
````



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | 表布局。 |
|
|  | 名称 | java.lang.String | 表名称。 |
|
|  | pageIndex | java.lang.Integer | 模板表所在页面的索引；如果模板表位于任意页面，则为  null  。 |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)
```


使用大写名称初始化 [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | 表布局。 |
|
|  | 名称 | java.lang.String | 表名称。 |
|
|  | pageIndex | java.lang.Integer | 模板表所在页面的索引；如果模板表位于任意页面，则为  null  。 |
|
|  | pageWidth | java.lang.Double | 用于创建模板项的页面宽度。 |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)
```


初始化 [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | 表布局。 |
|
|  | 名称 | java.lang.String | 表名称。 |
|
|  | pageIndex | java.lang.Integer | 模板表所在页面的索引；如果模板表位于任意页面，则为  null  。 |
|
|  | useUpperCaseName | boolean | 指示是否将  名称  转换为大写的值。 |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


初始化 [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | 表布局。 |
|
|  | 名称 | java.lang.String | 表名称。 |
|
|  | pageIndex | java.lang.Integer | 模板表所在页面的索引；如果模板表位于任意页面，则为  null  。 |
|
|  | pageWidth | java.lang.Double | 用于创建模板项的页面宽度。 |
|
|  | useUpperCaseName | boolean | 指示是否将  名称  转换为大写的值。 |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)
```


使用大写名称初始化 [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 类的新实例。

如果通过检测器参数设置了模板表，则表会自动检测：

````
TemplateTableParameters parameters = new TemplateTableParameters(
     new Rectangle(new Point(175, 350), new Size(400, 200)),
     java.util.Arrays.asList(new Double[] { 185.0, 370.0, 425.0, 485.0, 545.0 }));
 TemplateTable table = new TemplateTable(parameters, "Details", 0);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
 
````



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | 用于在自动模式下检测表的参数。 |
|
|  | 名称 | java.lang.String | 表名称。 |
|
|  | pageIndex | java.lang.Integer | 模板表所在页面的索引；如果模板表位于任意页面，则为  null  。 |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)
```


初始化 [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | 用于在自动模式下检测表的参数。 |
|
|  | 名称 | java.lang.String | 表名称。 |
|
|  | pageIndex | java.lang.Integer | 模板表所在页面的索引；如果模板表位于任意页面，则为  null  。 |
|
|  | pageWidth | java.lang.Double | 用于创建模板项的页面宽度。 |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)
```


初始化 [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | 用于在自动模式下检测表的参数。 |
|
|  | 名称 | java.lang.String | 表名称。 |
|
|  | pageIndex | java.lang.Integer | 模板表所在页面的索引；如果模板表位于任意页面，则为  null  。 |
|
|  | useUpperCaseName | boolean | 指示是否将  名称  转换为大写的值。 |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


初始化 [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | 用于在自动模式下检测表的参数。 |
|
|  | 名称 | java.lang.String | 表名称。 |
|
|  | pageIndex | java.lang.Integer | 模板表所在页面的索引；如果模板表位于任意页面，则为  null  。 |
|
|  | pageWidth | java.lang.Double | 用于创建模板项的页面宽度。 |
|
|  | useUpperCaseName | boolean | 指示是否将  名称  转换为大写的值。 |
|

### getLayout() {#getLayout--}
```
public TemplateTableLayout getLayout()
```


获取表布局。


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instance of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class that represents the table layout;  null  if it isn't set.

### getParameters() {#getParameters--}
```
public TemplateTableParameters getParameters()
```


获取自动模式下检测表的参数。


**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - An instance of  TemplateTableParameters  class that represents the parameters to detect the table in the automatic mode;  null  if it isn't set.

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

---
title: "TemplateRegexPosition"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供使用正则表达式的模板字段位置。"
type: docs
weight: 19
url: /zh/java/com.groupdocs.parser.templates/templateregexposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateRegexPosition extends TemplatePosition
```

提供使用正则表达式的模板字段位置。

以下示例展示了当文档包含 "Invoice Number INV-12345" 时的情况
然后可以按以下方式定义模板字段：

````
// Create a regex template field with "InvoiceNumber" name
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+[A-Z0-9\\-]+"),
     "InvoiceNumber");
 
````

在这种情况下，整个字符串被提取为值。若要仅提取字符串的一部分
使用正则表达式组 "value"：

````
// Create a regex template field with "InvoiceNumber" name with "value" group
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+(?[A-Z0-9\\-]+)"),
     "InvoiceNumber");
````

在这种情况下，提取的值为 "INV-3337" 字符串。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [TemplateRegexPosition(String expression)](#TemplateRegexPosition-java.lang.String-) | 初始化 [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition) 类的新实例。 |
|
|  | [TemplateRegexPosition(String expression, boolean matchCase)](#TemplateRegexPosition-java.lang.String-boolean-) | 初始化 [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getExpression()](#getExpression--) | 获取正则表达式。 |
|
|  | [isMatchCase()](#isMatchCase--) | 获取指示文本大小写是否未被忽略的值。 |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateRegexPosition(String expression) {#TemplateRegexPosition-java.lang.String-}
```
public TemplateRegexPosition(String expression)
```


初始化 [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | expression | java.lang.String | 正则表达式。 |
|

### TemplateRegexPosition(String expression, boolean matchCase) {#TemplateRegexPosition-java.lang.String-boolean-}
```
public TemplateRegexPosition(String expression, boolean matchCase)
```


初始化 [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | expression | java.lang.String | 正则表达式。 |
|
|  | matchCase | boolean | 指示文本大小写是否未被忽略的值。 |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


获取正则表达式。


**Returns:**
java.lang.String - 表示正则表达式的字符串。

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


获取指示文本大小写是否未被忽略的值。


**Returns:**
boolean -  true  如果文本大小写未被忽略；否则，  false 。

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

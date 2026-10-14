---
title: "FieldData"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示字段数据，例如名称、页面索引、字段值等。"
type: docs
weight: 13
url: /zh/java/com.groupdocs.parser.data/fielddata/
---
**Inheritance:**
java.lang.Object
```
public class FieldData
```

表示字段数据，例如名称、页面索引、字段值等。根据字段的不同，值可以是文本、图像、表格等。

在 [DocumentData](../../com.groupdocs.parser.data/documentdata) 集合中使用 [FieldData](../../com.groupdocs.parser.data/fielddata) 类的实例。

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getName()](#getName--) | 获取字段名称。 |
|
|  | [getPageIndex()](#getPageIndex--) | 获取页面索引。 |
|
|  | [getPageArea()](#getPageArea--) | 获取字段的值。 |
|
|  | [getLinkedField()](#getLinkedField--) | 获取链接的字段。 |
|
|  | [getText()](#getText--) | 获取文本。 |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | 获取一个值，指示是否已将  名称  转换为大写。 |
|
### getName() {#getName--}
```
public String getName()
```


获取字段名称。


**Returns:**
java.lang.String - 表示字段名称的全大写字符串值。

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


获取页面索引。


**Returns:**
int - 包含该字段的页面的零基索引。

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


获取字段的值。

根据字段，PageArea 属性可以包含 [PageArea](../../com.groupdocs.parser.data/pagearea) 类的任何子类。
例如，[Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) 方法仅提取文本字段。

````
PageTextArea area = field.getPageArea() instanceof PageTextArea
         ? (PageTextArea) field.getPageArea()
         : null;
 System.out.println(area == null ? "Not a template field" : area.getText());
 
````



**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - An instance of [PageArea](../../com.groupdocs.parser.data/pagearea) class that represents the value of the field.

### getLinkedField() {#getLinkedField--}
```
public FieldData getLinkedField()
```


获取链接的字段。


**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class that represents the field which is linked to the field;  null  if it isn't set.

### getText() {#getText--}
```
public String getText()
```


获取文本。


**Returns:**
java.lang.String - 表示字段 text 值的字符串；如果 [PageArea](../../com.groupdocs.parser.data/pagearea) 属性不是 [PageTextArea](../../com.groupdocs.parser.data/pagetextarea)，则为 null。

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


获取一个值，指示是否已将  名称  转换为大写。


**Returns:**
boolean - 一个布尔值，指示是否已将  名称  转换为大写。


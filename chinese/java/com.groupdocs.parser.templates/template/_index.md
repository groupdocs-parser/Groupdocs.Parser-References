---
title: "Template"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供文档页面模板。"
type: docs
weight: 10
url: /zh/java/com.groupdocs.parser.templates/template/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Template implements Iterable<TemplateItem>
```

提供文档页面模板。它由 [TemplateItem](../../com.groupdocs.parser.templates/templateitem) 对象组成，这些对象表示模板的项目，如文本字段和表格定义。

**Learn more:**

* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [Template(Iterable<? extends TemplateItem> items)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--) | 初始化一个新的 [Template](../../com.groupdocs.parser.templates/template) 类实例。 |
|
|  | [Template(Iterable<? extends TemplateItem> items, TemplateOptions options)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-) | 初始化一个新的 [Template](../../com.groupdocs.parser.templates/template) 类实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getCount()](#getCount--) | 获取模板项目的总数。 |
|
|  | [get(int index)](#get-int-) | 通过索引获取模板项目。 |
|
|  | [getOptions()](#getOptions--) | 获取模板选项。 |
|
| [iterator()](#iterator--) |  |
|  | [load(String filePath)](#load-java.lang.String-) | 从文件加载模板。 |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | 从流加载模板。 |
|
|  | [save(String filePath)](#save-java.lang.String-) | 将模板保存到文件。 |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | 将模板保存到流。 |
|
### Template(Iterable<? extends TemplateItem> items) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--}
```
public Template(Iterable<? extends TemplateItem> items)
```


初始化一个新的 [Template](../../com.groupdocs.parser.templates/template) 类实例。

用法：

````
// Create an array of template fields
 TemplateItem[] fields = new TemplateItem[]
 {
     new TemplateField(new TemplateRegexPosition("From"), "From", 0),
     new TemplateField(
         new TemplateLinkedPosition("From", new Size(100, 10), new TemplateLinkedPositionEdges(false, false, false, true)),
         "FromCompany",
         0),
     new TemplateField(
         new TemplateLinkedPosition("FromCompany", new Size(100, 30), new TemplateLinkedPositionEdges(false, false, false, true)),
         "FromAddress",
         0)
 };
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(fields));
 
````



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | 包含 [TemplateItem](../../com.groupdocs.parser.templates/templateitem) 对象的集合。 |
|

### Template(Iterable<? extends TemplateItem> items, TemplateOptions options) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-}
```
public Template(Iterable<? extends TemplateItem> items, TemplateOptions options)
```


初始化一个新的 [Template](../../com.groupdocs.parser.templates/template) 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | 包含 [TemplateItem](../../com.groupdocs.parser.templates/templateitem) 对象的集合。 |
|
|  | options | [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) | 模板选项。 |
|

### getCount() {#getCount--}
```
public int getCount()
```


获取模板项目的总数。


**Returns:**
int - 表示模板项目总数的整数。

### get(int index) {#get-int-}
```
public TemplateItem get(int index)
```


通过索引获取模板项目。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 索引 | int | 模板项的零基索引。 |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - An instance of [TemplateItem](../../com.groupdocs.parser.templates/templateitem) class.

### getOptions() {#getOptions--}
```
public TemplateOptions getOptions()
```


获取模板选项。


**Returns:**
[TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) - An instance of [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) class.

### iterator() {#iterator--}
```
public Iterator<TemplateItem> iterator()
```




**Returns:**
java.util.Iterator<com.groupdocs.parser.templates.TemplateItem>
### load(String filePath) {#load-java.lang.String-}
```
public static Template load(String filePath)
```


从文件加载模板。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | filePath | java.lang.String | 文件的路径。 |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Template load(InputStream stream)
```


从流加载模板。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | stream | java.io.InputStream | 输入流。 |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


将模板保存到文件。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | filePath | java.lang.String | 文件的路径。 |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


将模板保存到流。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | stream | java.io.OutputStream | 输出流。 |
|


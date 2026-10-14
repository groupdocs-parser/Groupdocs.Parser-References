---
title: "DocumentData"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示文档的数据。"
type: docs
weight: 11
url: /zh/java/com.groupdocs.parser.data/documentdata/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class DocumentData implements Iterable<FieldData>
```

表示文档的数据。它由包含文档字段数据的 [FieldData](../../com.groupdocs.parser.data/fielddata) 对象组成。 [DocumentData](../../com.groupdocs.parser.data/documentdata) 类的实例用作 [Parser.parseByTemplate(Template)](../../com.groupdocs.parser/parser#parseByTemplate-Template-) 和 [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) 方法的返回值。请参阅那里的使用示例。

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getTemplate()](#getTemplate--) | 获取生成此文档数据的模板。 |
|
|  | [getCount()](#getCount--) | 获取字段数据的总数。 |
|
|  | [get(int index)](#get-int-) | 通过索引获取字段数据。 |
|
|  | [getFieldsByName(String fieldName)](#getFieldsByName-java.lang.String-) | 返回名称等于  fieldName  的字段数据集合。 |
|
|  | [iterator()](#iterator--) | 返回此列表中元素的迭代器，按正确顺序。 |
|
### getTemplate() {#getTemplate--}
```
public Template getTemplate()
```


获取生成此文档数据的模板。

当数据是通过自动模板集合选择生成时（参见
[Parser.parseByTemplate(com.groupdocs.parser.templates.TemplateCollection, com.groupdocs.parser.options.ParseByTemplateOptions)](../../com.groupdocs.parser/parser#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection--com.groupdocs.parser.options.ParseByTemplateOptions-)),
这是所选模板。
null
当数据不是由模板生成时。


**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - The source [Template](../../com.groupdocs.parser.templates/template), or  null .

### getCount() {#getCount--}
```
public int getCount()
```


获取字段数据的总数。


**Returns:**
int - 表示字段数据总数的整数值。

### get(int index) {#get-int-}
```
public FieldData get(int index)
```


通过索引获取字段数据。

遍历所有字段：

````
// Print all extracted data
 for (int i = 0; i < data.getCount(); i++) {
     // Print field name
     System.out.print(data.get(i).getName() + ": ");
     // As we have defined only text fields in the template,
     // we cast PageArea property value to PageTextArea
     PageTextArea area = data.get(i).getPageArea() instanceof PageTextArea
             ? (PageTextArea) data.get(i).getPageArea()
             : null;
     System.out.println(area == null ? "Not a template field" : area.getText());
 }
 
````

[FieldData](../../com.groupdocs.parser.data/fielddata) class represents field data. Depending on the field PageArea property can contain any
继承自 [PageArea](../../com.groupdocs.parser.data/pagearea) 类的子类。例如， [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) 方法仅提取文本字段：

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleFormsPdf)) {
     // Extract data from PDF document
     DocumentData data = parser.parseForm();
     // Check if form extraction is supported
     if (data == null) {
         System.out.println("Form extraction isn't supported.");
         return;
     }
     // Iterate over extracted data
     for (int i = 0; i < data.getCount(); i++) {
         System.out.print(data.get(i).getName() + ": ");
         PageTextArea area = data.get(i).getPageArea() instanceof PageTextArea
                 ? (PageTextArea) data.get(i).getPageArea()
                 : null;
         System.out.println(area == null ? "Not a template field" : area.getText());
     }
 }
 
````



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 索引 | int | 字段的零基索引。 |
|

**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class.

### getFieldsByName(String fieldName) {#getFieldsByName-java.lang.String-}
```
public List<FieldData> getFieldsByName(String fieldName)
```


返回名称等于  fieldName  的字段数据集合。

按字段名称查找字段：

````
// Print prices
 System.out.println("Prices:");
 for (FieldData field : data.getFieldsByName("Price")) {
     PageTextArea area = field.getPageArea() instanceof PageTextArea
             ? (PageTextArea) field.getPageArea()
             : null;
     System.out.println(area == null ? "Not a template field" : area.getText());
 }
 
````

[FieldData](../../com.groupdocs.parser.data/fielddata) class represents field data. Depending on the field [PageArea](../../com.groupdocs.parser.data/pagearea) property can contain
任意继承自 [PageArea](../../com.groupdocs.parser.data/pagearea) 类的子类。例如， [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) 方法仅提取文本字段。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | fieldName | java.lang.String | 字段的名称。 |
|

**Returns:**
java.util.List<com.groupdocs.parser.data.FieldData> - 一个包含 [FieldData](../../com.groupdocs.parser.data/fielddata) 对象的集合；如果未找到字段数据，则为空集合。

### iterator() {#iterator--}
```
public Iterator<FieldData> iterator()
```


返回此列表中元素的迭代器，按正确顺序。


**Returns:**
java.util.Iterator<com.groupdocs.parser.data.FieldData> - 一个按正确顺序遍历此列表中元素的迭代器。


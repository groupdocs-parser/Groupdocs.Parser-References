---
title: "TocItem"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示在目录提取功能中使用的项。"
type: docs
weight: 31
url: /zh/java/com.groupdocs.parser.data/tocitem/
---
**Inheritance:**
java.lang.Object
```
public class TocItem
```

表示在目录提取功能中使用的项。

[TocItem](../../com.groupdocs.parser.data/tocitem) 类的实例用作 [Parser.getToc()](../../com.groupdocs.parser/parser#getToc--) 方法的返回值。请参阅那里的使用示例。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [TocItem(int depth, String text, Integer pageIndex)](#TocItem-int-java.lang.String-java.lang.Integer-) | 初始化一个新的 TocItem 类实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getDepth()](#getDepth--) | 获取深度级别。 |
|
|  | [getText()](#getText--) | 获取文本。 |
|
|  | [getPageIndex()](#getPageIndex--) | 获取页面索引。 |
|
|  | [extractText()](#extractText--) | 提取 TocItem 对象所引用的文档中的文本。 |
|
### TocItem(int depth, String text, Integer pageIndex) {#TocItem-int-java.lang.String-java.lang.Integer-}
```
public TocItem(int depth, String text, Integer pageIndex)
```


初始化一个新的 TocItem 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | depth | int | 该项的深度级别。 |
|
|  | 文本 | java.lang.String | 该项的文本。 |
|
|  | pageIndex | java.lang.Integer | 该项引用的页索引 |
|

### getDepth() {#getDepth--}
```
public int getDepth()
```


获取深度级别。


**Returns:**
int - 表示该项深度级别的整数值。

### getText() {#getText--}
```
public String getText()
```


获取文本。


**Returns:**
java.lang.String - 表示该项文本的字符串值。

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


获取页面索引。


**Returns:**
java.lang.Integer - 表示该项引用的页索引的整数值；如果未设置，则为 null。

### extractText() {#extractText--}
```
public TextReader extractText()
```


提取 TocItem 对象所引用的文档中的文本。

以下示例演示如何通过目录项提取文本：

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleDocxWithToc)) {
     // Get table of contents
     Iterable tocItems = parser.getToc();

     // Check if toc extraction is supported
     if (tocItems == null) {
         System.out.println("Table of contents extraction isn't supported");
     }

     // Iterate over items
     for (TocItem tocItem : tocItems) {
         // Print the text of the chapter
         try (TextReader reader = tocItem.extractText()) {
             System.out.println("----");
             System.out.println(reader.readToEnd());
         }
     }
 }
 
````



**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text.


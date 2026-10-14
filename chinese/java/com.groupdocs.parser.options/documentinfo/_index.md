---
title: "DocumentInfo"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示文档信息。"
type: docs
weight: 11
url: /zh/java/com.groupdocs.parser.options/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.parser.options.IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo)
```
public abstract class DocumentInfo implements IDocumentInfo
```

表示文档信息。

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getFileType()](#getFileType--) | 获取文档类型。 |
|
|  | [getPageCount()](#getPageCount--) | 获取文档页面的总数。 |
|
|  | [getRawPageCount()](#getRawPageCount--) | 获取文档原始页面的总数。 |
|
|  | [getSize()](#getSize--) | 获取文档的字节大小。 |
|
|  | [getPages()](#getPages--) | 获取有关页面的信息，例如索引和页面大小。 |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


获取文档类型。


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getPageCount() {#getPageCount--}
```
public abstract int getPageCount()
```


获取文档页面的总数。


**Returns:**
int - 表示页面总数的整数值。

### getRawPageCount() {#getRawPageCount--}
```
public abstract int getRawPageCount()
```


获取文档原始页面的总数。

在原始文本提取时，使用 [getRawPageCount()](../../com.groupdocs.parser.options/documentinfo#getRawPageCount--) 属性而不是 [getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) 属性。
某些文档在精确和原始文本提取模式下的页码不同。
[getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) property may perform extra calculations which impacts on text extraction speed in raw mode.


**Returns:**
int - 表示原始页面总数的整数值。

### getSize() {#getSize--}
```
public abstract long getSize()
```


获取文档的字节大小。


**Returns:**
long - 表示文档字节大小的整数值。

### getPages() {#getPages--}
```
public abstract List<PageInfo> getPages()
```


获取有关页面的信息，例如索引和页面大小。


**Returns:**
java.util.List<com.groupdocs.parser.options.PageInfo> - 包含 [PageInfo](../../com.groupdocs.parser.options/pageinfo) 类实例的集合。


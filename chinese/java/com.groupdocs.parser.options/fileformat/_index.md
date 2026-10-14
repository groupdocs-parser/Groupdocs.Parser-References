---
title: "FileFormat"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "定义文件的类型。"
type: docs
weight: 43
url: /zh/java/com.groupdocs.parser.options/fileformat/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum FileFormat extends Enum<FileFormat>
```

定义文件的类型。

**Learn more:**

* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)

## 字段

| 字段 | 描述 |
| --- | --- |
|  | [Unknown](#Unknown) | 默认值。 |
|
|  | [WordProcessing](#WordProcessing) | 文字处理文档（DOC、DOCX、ODT 等）。 |
|
|  | [Spreadsheet](#Spreadsheet) | 电子表格文档（XLS、XLSX、ODS 等）。 |
|
|  | [Presentation](#Presentation) | 演示文稿文档（PPT、PPTX、ODP 等）。 |
|
|  | [Email](#Email) | 电子邮件文档（电子邮件消息或电子邮件容器）。 |
|
|  | [Pdf](#Pdf) | PDF 文档。 |
|
|  | [Markup](#Markup) | 标记文档（HTML、XML、Markdown 等）。 |
|
|  | [Ebook](#Ebook) | 电子书文档（ePUB、FictionBook 等）。 |
|
|  | [Note](#Note) | 笔记文档。 |
|
|  | [Archive](#Archive) | 归档文件。 |
|
|  | [Database](#Database) | 数据库文件（通过 JDBC）。 |
|
|  | [Image](#Image) | 图像文件。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Unknown {#Unknown}
```
public static final FileFormat Unknown
```


默认值。


### WordProcessing {#WordProcessing}
```
public static final FileFormat WordProcessing
```


文字处理文档（DOC、DOCX、ODT 等）。


### Spreadsheet {#Spreadsheet}
```
public static final FileFormat Spreadsheet
```


电子表格文档（XLS、XLSX、ODS 等）。


### Presentation {#Presentation}
```
public static final FileFormat Presentation
```


演示文稿文档（PPT、PPTX、ODP 等）。


### Email {#Email}
```
public static final FileFormat Email
```


电子邮件文档（电子邮件消息或电子邮件容器）。


### Pdf {#Pdf}
```
public static final FileFormat Pdf
```


PDF 文档。


### Markup {#Markup}
```
public static final FileFormat Markup
```


标记文档（HTML、XML、Markdown 等）。


### Ebook {#Ebook}
```
public static final FileFormat Ebook
```


电子书文档（ePUB、FictionBook 等）。


### Note {#Note}
```
public static final FileFormat Note
```


笔记文档。


### Archive {#Archive}
```
public static final FileFormat Archive
```


归档文件。


### Database {#Database}
```
public static final FileFormat Database
```


数据库文件（通过 JDBC）。


### Image {#Image}
```
public static final FileFormat Image
```


图像文件。


### values() {#values--}
```
public static FileFormat[] values()
```




**Returns:**
com.groupdocs.parser.options.FileFormat[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static FileFormat valueOf(String name)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat)

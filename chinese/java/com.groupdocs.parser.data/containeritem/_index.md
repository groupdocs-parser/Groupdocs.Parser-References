---
title: "ContainerItem"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示容器项，例如 Zip 存档实体、电子邮件附件、PDF 作品集项等。"
type: docs
weight: 10
url: /zh/java/com.groupdocs.parser.data/containeritem/
---
**Inheritance:**
java.lang.Object
```
public abstract class ContainerItem
```

表示容器项，例如 Zip 存档实体、电子邮件附件、PDF Portfolio 项等。

一个 [ContainerItem](../../com.groupdocs.parser.data/containeritem) 类的实例用作 [Parser.getContainer()](../../com.groupdocs.parser/parser#getContainer--) 方法的返回值。请参阅那里的使用示例。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | 使用项目名称和目录初始化一个新的 [ContainerItem](../../com.groupdocs.parser.data/containeritem) 实例。 |
|
|  | [ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | 使用项目完整路径初始化一个新的 [ContainerItem](../../com.groupdocs.parser.data/containeritem) 实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getName()](#getName--) | 获取项目的名称。 |
|
|  | [getDirectory()](#getDirectory--) | 获取项目的目录。 |
|
|  | [getFilePath()](#getFilePath--) | 获取项目的完整路径。 |
|
|  | [getSize()](#getSize--) | 获取项目的大小。 |
|
|  | [getMetadata()](#getMetadata--) | 获取元数据项的集合。 |
|
|  | [getMetadataValue(String name)](#getMetadataValue-java.lang.String-) | 获取元数据值。 |
|
|  | [openStream()](#openStream--) | 打开项目内容的流。 |
|
|  | [openParser()](#openParser--) | 为项目内容创建 [Parser](../../com.groupdocs.parser/parser) 对象。 |
|
|  | [openParser(LoadOptions loadOptions)](#openParser-com.groupdocs.parser.options.LoadOptions-) | 创建用于项目内容的 [Parser](../../com.groupdocs.parser/parser) 对象，并使用 [LoadOptions](../../com.groupdocs.parser.options/loadoptions)。 |
|
|  | [openParser(LoadOptions loadOptions, ParserSettings parserSettings)](#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | 创建用于项目内容的 [Parser](../../com.groupdocs.parser/parser) 对象，使用 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 和 [ParserSettings](../../com.groupdocs.parser.options/parsersettings)。 |
|
|  | [detectFileType(FileTypeDetectionMode detectionMode)](#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-) | 检测容器项目的文件类型。 |
|
### ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)
```


使用项目名称和目录初始化一个新的 [ContainerItem](../../com.groupdocs.parser.data/containeritem) 实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 名称 | java.lang.String | 项目的名称。 |
|
|  | 目录 | java.lang.String | 项目的目录。 |
|
|  | size | long | 项目的大小。 |
|
|  | 元数据 | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | 元数据项的集合。 |
|

### ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)
```


使用项目完整路径初始化一个新的 [ContainerItem](../../com.groupdocs.parser.data/containeritem) 实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | filePath | java.lang.String | 项目的完整路径。 |
|
|  | size | long | 项目的大小。 |
|
|  | 元数据 | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | 元数据项的集合。 |
|

### getName() {#getName--}
```
public String getName()
```


获取项目的名称。


**Returns:**
java.lang.String - 表示项目文件名（不含目录）的字符串值。

### getDirectory() {#getDirectory--}
```
public String getDirectory()
```


获取项目的目录。


**Returns:**
java.lang.String - 表示项目目录（不含文件名）的字符串值。

### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


获取项目的完整路径。


**Returns:**
java.lang.String - 表示项目完整路径的字符串值。

### getSize() {#getSize--}
```
public long getSize()
```


获取项目的大小。


**Returns:**
long - 表示项目大小（以字节为单位）的整数值。

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


获取元数据项的集合。


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - [MetadataItem](../../com.groupdocs.parser.data/metadataitem) 对象的集合；如果未设置元数据则为空。

### getMetadataValue(String name) {#getMetadataValue-java.lang.String-}
```
public String getMetadataValue(String name)
```


获取元数据值。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 名称 | java.lang.String | 元数据的名称。 |
|

**Returns:**
java.lang.String - 表示元数据项值的字符串；如果未找到具有此名称的元数据，则为 null。

### openStream() {#openStream--}
```
public abstract InputStream openStream()
```


打开项目内容的流。


**Returns:**
java.io.InputStream - 包含项目内容的流。

### openParser() {#openParser--}
```
public Parser openParser()
```


为项目内容创建 [Parser](../../com.groupdocs.parser/parser) 对象。


**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions) {#openParser-com.groupdocs.parser.options.LoadOptions-}
```
public Parser openParser(LoadOptions loadOptions)
```


创建用于项目内容的 [Parser](../../com.groupdocs.parser/parser) 对象，并使用 [LoadOptions](../../com.groupdocs.parser.options/loadoptions)。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | 打开项目内容的选项。 |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions, ParserSettings parserSettings) {#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public abstract Parser openParser(LoadOptions loadOptions, ParserSettings parserSettings)
```


创建用于项目内容的 [Parser](../../com.groupdocs.parser/parser) 对象，使用 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 和 [ParserSettings](../../com.groupdocs.parser.options/parsersettings)。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | 打开项目内容的选项。 |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | 用于自定义数据提取的解析器设置。 |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### detectFileType(FileTypeDetectionMode detectionMode) {#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-}
```
public abstract FileType detectFileType(FileTypeDetectionMode detectionMode)
```


检测容器项目的文件类型。


检测模式
参数提供控制文件类型检测的能力：

* **Default**. The file type is detected by the file extension; if the file extension isn't recognized, the file type is detected by the file content.
* **Extension**.The file type is detected only by the file extension.
* **Content**. The file type is detected only by the file content.

以下示例展示了如何检测容器项目的文件类型：

````
// Create an instance of Parser class
 try (Parser parser = new Parser(filePath)) {
     // Extract attachments from the container
     Iterable attachments = parser.getContainer();
     // Check if container extraction is supported
     if (attachments == null) {
         System.out.println("Container extraction isn't supported");
     }
     // Iterate over attachments
     for (ContainerItem item : attachments) {
         // Detect the file type
         FileType fileType = item.detectFileType(FileTypeDetectionMode.Default);
         // Print the name and file type
         System.out.println(String.format("%s: %s", item.getName(), fileType));
     }
 }
 
````



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | detectionMode | [FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode) | 定义文件类型检测的模式。 |
|

**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class; [FileType.Unknown](../../com.groupdocs.parser.options/filetype#Unknown) if a file type isn't detected.


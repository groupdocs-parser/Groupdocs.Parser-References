---
title: ContainerItem
second_title: GroupDocs.Parser for Java API Reference
description: Represents a container item like Zip archive entity email attachment PDF Portfolio item and so on.
type: docs
weight: 10
url: /java/com.groupdocs.parser.data/containeritem/
---
**Inheritance:**
java.lang.Object
```
public abstract class ContainerItem
```

Represents a container item like Zip archive entity, email attachment, PDF Portfolio item and so on.

An instance of [ContainerItem](../../com.groupdocs.parser.data/containeritem) class is used as return value of [Parser.getContainer()](../../com.groupdocs.parser/parser\#getContainer--) method. See the usage examples there.
## Constructors

| Constructor | Description |
| --- | --- |
| [ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | Initializes a new instance of [ContainerItem](../../com.groupdocs.parser.data/containeritem) with the item name and directory. |
| [ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | Initializes a new instance of [ContainerItem](../../com.groupdocs.parser.data/containeritem) with the item full path. |
## Methods

| Method | Description |
| --- | --- |
| [getName()](#getName--) | Gets the name of the item. |
| [getDirectory()](#getDirectory--) | Gets the directory of the item. |
| [getFilePath()](#getFilePath--) | Gets the full path of the item. |
| [getSize()](#getSize--) | Gets the size of the item. |
| [getMetadata()](#getMetadata--) | Gets the collection of metadata items. |
| [openStream()](#openStream--) | Opens the stream of the item content. |
| [openParser()](#openParser--) | Creates the [Parser](../../com.groupdocs.parser/parser) object for the item content. |
| [openParser(LoadOptions loadOptions)](#openParser-com.groupdocs.parser.options.LoadOptions-) | Creates the [Parser](../../com.groupdocs.parser/parser) object for the item content with [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
| [openParser(LoadOptions loadOptions, ParserSettings parserSettings)](#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Creates the [Parser](../../com.groupdocs.parser/parser) object for the item content with [LoadOptions](../../com.groupdocs.parser.options/loadoptions) and [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
| [detectFileType(FileTypeDetectionMode detectionMode)](#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-) | Detects a file type of the container item. |
### ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)
```


Initializes a new instance of [ContainerItem](../../com.groupdocs.parser.data/containeritem) with the item name and directory.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the item. |
| directory | java.lang.String | The directory of the item. |
| size | long | The size of the item. |
| metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | The collection of metadata items. |

### ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)
```


Initializes a new instance of [ContainerItem](../../com.groupdocs.parser.data/containeritem) with the item full path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The full path of the item. |
| size | long | The size of the item. |
| metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | The collection of metadata items. |

### getName() {#getName--}
```
public String getName()
```


Gets the name of the item.

**Returns:**
java.lang.String - A string value that represents the file name of the item (without a directory).
### getDirectory() {#getDirectory--}
```
public String getDirectory()
```


Gets the directory of the item.

**Returns:**
java.lang.String - A string value that represents the directory of the item (without a file name).
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Gets the full path of the item.

**Returns:**
java.lang.String - A string value that represents the full path of the item.
### getSize() {#getSize--}
```
public long getSize()
```


Gets the size of the item.

**Returns:**
long - An integer value that represents the size of the item in bytes.
### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


Gets the collection of metadata items.

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - A collection of [MetadataItem](../../com.groupdocs.parser.data/metadataitem) objects; empty if metadata isn't set.
### openStream() {#openStream--}
```
public abstract InputStream openStream()
```


Opens the stream of the item content.

**Returns:**
java.io.InputStream - A stream with the item content.
### openParser() {#openParser--}
```
public Parser openParser()
```


Creates the [Parser](../../com.groupdocs.parser/parser) object for the item content.

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.
### openParser(LoadOptions loadOptions) {#openParser-com.groupdocs.parser.options.LoadOptions-}
```
public Parser openParser(LoadOptions loadOptions)
```


Creates the [Parser](../../com.groupdocs.parser/parser) object for the item content with [LoadOptions](../../com.groupdocs.parser.options/loadoptions).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | The options to open the item content. |

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.
### openParser(LoadOptions loadOptions, ParserSettings parserSettings) {#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public abstract Parser openParser(LoadOptions loadOptions, ParserSettings parserSettings)
```


Creates the [Parser](../../com.groupdocs.parser/parser) object for the item content with [LoadOptions](../../com.groupdocs.parser.options/loadoptions) and [ParserSettings](../../com.groupdocs.parser.options/parsersettings).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | The options to open the item content. |
| parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | The parser settings which are used to customize data extraction. |

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.
### detectFileType(FileTypeDetectionMode detectionMode) {#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-}
```
public abstract FileType detectFileType(FileTypeDetectionMode detectionMode)
```


Detects a file type of the container item.

 detectionMode  parameter provides the ability to control file type detection:

 *  **Default**. The file type is detected by the file extension; if the file extension isn't recognized, the file type is detected by the file content.
 *  **Extension**.The file type is detected only by the file extension.
 *  **Content**. The file type is detected only by the file content.

The following example shows how to detect file type of container item:

```
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
 
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| detectionMode | [FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode) | Defines a mode of the file type detection. |

**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class; [FileType.Unknown](../../com.groupdocs.parser.options/filetype\#Unknown) if a file type isn't detected.

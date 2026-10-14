---
title: "FileInfo"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示文件信息。"
type: docs
weight: 19
url: /zh/java/com.groupdocs.parser.options/fileinfo/
---
**Inheritance:**
java.lang.Object
```
public class FileInfo
```

表示文件信息。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [FileInfo(FileType fileType, long size, boolean encrypted)](#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getFileType()](#getFileType--) | 获取文档类型。 |
|
|  | [getSize()](#getSize--) | 获取文档的字节大小。 |
|
|  | [isEncrypted()](#isEncrypted--) | 获取表示文件是否受密码保护的值。 |
|
### FileInfo(FileType fileType, long size, boolean encrypted) {#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-}
```
public FileInfo(FileType fileType, long size, boolean encrypted)
```


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileType | [FileType](../../com.groupdocs.parser.options/filetype) |  |
| size | long |  |
| encrypted | boolean |  |

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


获取文档类型。


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getSize() {#getSize--}
```
public long getSize()
```


获取文档的字节大小。


**Returns:**
long - 表示文档字节大小的整数值。

### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


获取表示文件是否受密码保护的值。


**Returns:**
boolean - 如果文件受密码保护则为 true；否则为 false。


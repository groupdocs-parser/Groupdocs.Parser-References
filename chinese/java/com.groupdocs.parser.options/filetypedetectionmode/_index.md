---
title: "FileTypeDetectionMode"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "定义文件类型检测的模式。"
type: docs
weight: 44
url: /zh/java/com.groupdocs.parser.options/filetypedetectionmode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum FileTypeDetectionMode extends Enum<FileTypeDetectionMode>
```

定义文件类型检测的模式。

## 字段

| 字段 | 描述 |
| --- | --- |
|  | [Default](#Default) | 文件类型通过文件扩展名检测；如果文件扩展名未被识别，则通过文件内容检测文件类型。 |
|
|  | [Extension](#Extension) | 文件类型仅通过文件扩展名检测。 |
|
|  | [Content](#Content) | 文件类型仅通过文件内容检测。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Default {#Default}
```
public static final FileTypeDetectionMode Default
```


文件类型通过文件扩展名检测；如果文件扩展名未被识别，则通过文件内容检测文件类型。


### Extension {#Extension}
```
public static final FileTypeDetectionMode Extension
```


文件类型仅通过文件扩展名检测。


### Content {#Content}
```
public static final FileTypeDetectionMode Content
```


文件类型仅通过文件内容检测。


### values() {#values--}
```
public static FileTypeDetectionMode[] values()
```




**Returns:**
com.groupdocs.parser.options.FileTypeDetectionMode[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static FileTypeDetectionMode valueOf(String name)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode)

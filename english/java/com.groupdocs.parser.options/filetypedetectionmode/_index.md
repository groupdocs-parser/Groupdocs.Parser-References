---
title: FileTypeDetectionMode
second_title: GroupDocs.Parser for Java API Reference
description: Defines a mode of the file type detection.
type: docs
weight: 43
url: /java/com.groupdocs.parser.options/filetypedetectionmode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum FileTypeDetectionMode extends Enum<FileTypeDetectionMode>
```

Defines a mode of the file type detection.
## Fields

| Field | Description |
| --- | --- |
| [Default](#Default) | The file type is detected by the file extension; if the file extension isn't recognized, the file type is detected by the file content. |
| [Extension](#Extension) | The file type is detected only by the file extension. |
| [Content](#Content) | The file type is detected only by the file content. |
## Methods

| Method | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Default {#Default}
```
public static final FileTypeDetectionMode Default
```


The file type is detected by the file extension; if the file extension isn't recognized, the file type is detected by the file content.

### Extension {#Extension}
```
public static final FileTypeDetectionMode Extension
```


The file type is detected only by the file extension.

### Content {#Content}
```
public static final FileTypeDetectionMode Content
```


The file type is detected only by the file content.

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
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode)

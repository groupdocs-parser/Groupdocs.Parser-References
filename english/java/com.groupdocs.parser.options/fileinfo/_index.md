---
title: FileInfo
second_title: GroupDocs.Parser for Java API Reference
description: Represents the file information.
type: docs
weight: 18
url: /java/com.groupdocs.parser.options/fileinfo/
---
**Inheritance:**
java.lang.Object
```
public class FileInfo
```

Represents the file information.
## Constructors

| Constructor | Description |
| --- | --- |
| [FileInfo(FileType fileType, long size, boolean encrypted)](#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-) |  |
## Methods

| Method | Description |
| --- | --- |
| [getFileType()](#getFileType--) | Gets the document type. |
| [getSize()](#getSize--) | Gets the size of the document in bytes. |
| [isEncrypted()](#isEncrypted--) | Gets a value that represents whether a file is password-protected. |
### FileInfo(FileType fileType, long size, boolean encrypted) {#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-}
```
public FileInfo(FileType fileType, long size, boolean encrypted)
```


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileType | [FileType](../../com.groupdocs.parser.options/filetype) |  |
| size | long |  |
| encrypted | boolean |  |

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Gets the document type.

**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.
### getSize() {#getSize--}
```
public long getSize()
```


Gets the size of the document in bytes.

**Returns:**
long - An integer value that represents the size of the document in bytes.
### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


Gets a value that represents whether a file is password-protected.

**Returns:**
boolean - A boolean true if a file is password-protected; otherwise false.

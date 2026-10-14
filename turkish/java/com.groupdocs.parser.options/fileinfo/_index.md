---
title: "FileInfo"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Dosya bilgisini temsil eder."
type: docs
weight: 19
url: /tr/java/com.groupdocs.parser.options/fileinfo/
---
**Inheritance:**
java.lang.Object
```
public class FileInfo
```

Dosya bilgisini temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [FileInfo(FileType fileType, long size, boolean encrypted)](#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getFileType()](#getFileType--) | Belge tipini alır. |
|
|  | [getSize()](#getSize--) | Belgenin bayt cinsinden boyutunu alır. |
|
|  | [isEncrypted()](#isEncrypted--) | Bir dosyanın şifre korumalı olup olmadığını temsil eden bir değeri alır. |
|
### FileInfo(FileType fileType, long size, boolean encrypted) {#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-}
```
public FileInfo(FileType fileType, long size, boolean encrypted)
```


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileType | [FileType](../../com.groupdocs.parser.options/filetype) |  |
| size | long |  |
| şifrelenmiş | boolean |  |

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Belge tipini alır.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getSize() {#getSize--}
```
public long getSize()
```


Belgenin bayt cinsinden boyutunu alır.


**Returns:**
long - Belge boyutunu bayt cinsinden temsil eden bir tam sayı değeri.

### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


Bir dosyanın şifre korumalı olup olmadığını temsil eden bir değeri alır.


**Returns:**
boolean - Dosya şifre korumalıysa doğru; aksi takdirde yanlış.


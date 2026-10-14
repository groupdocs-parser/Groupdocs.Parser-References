---
title: "FileInfo"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل معلومات الملف."
type: docs
weight: 19
url: /ar/java/com.groupdocs.parser.options/fileinfo/
---
**Inheritance:**
java.lang.Object
```
public class FileInfo
```

يمثل معلومات الملف.

## البناؤات

| البناء | الوصف |
| --- | --- |
| [FileInfo(FileType fileType, long size, boolean encrypted)](#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-) |  |
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getFileType()](#getFileType--) | يحصل على نوع المستند. |
|
|  | [getSize()](#getSize--) | يحصل على حجم المستند بالبايت. |
|
|  | [isEncrypted()](#isEncrypted--) | يحصل على قيمة تمثل ما إذا كان الملف محميًا بكلمة مرور. |
|
### FileInfo(FileType fileType, long size, boolean encrypted) {#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-}
```
public FileInfo(FileType fileType, long size, boolean encrypted)
```


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
| fileType | [FileType](../../com.groupdocs.parser.options/filetype) |  |
| size | long |  |
| encrypted | boolean |  |

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


يحصل على نوع المستند.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getSize() {#getSize--}
```
public long getSize()
```


يحصل على حجم المستند بالبايت.


**Returns:**
long - قيمة عدد صحيح تمثل حجم المستند بالبايت.

### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


يحصل على قيمة تمثل ما إذا كان الملف محميًا بكلمة مرور.


**Returns:**
boolean - قيمة منطقية true إذا كان الملف محميًا بكلمة مرور؛ وإلا false.


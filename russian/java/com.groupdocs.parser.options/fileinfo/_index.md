---
title: "FileInfo"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет информацию о файле."
type: docs
weight: 19
url: /ru/java/com.groupdocs.parser.options/fileinfo/
---
**Inheritance:**
java.lang.Object
```
public class FileInfo
```

Представляет информацию о файле.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [FileInfo(FileType fileType, long size, boolean encrypted)](#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getFileType()](#getFileType--) | Получает тип документа. |
|
|  | [getSize()](#getSize--) | Получает размер документа в байтах. |
|
|  | [isEncrypted()](#isEncrypted--) | Получает значение, представляющее, защищён ли файл паролем. |
|
### FileInfo(FileType fileType, long size, boolean encrypted) {#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-}
```
public FileInfo(FileType fileType, long size, boolean encrypted)
```


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileType | [FileType](../../com.groupdocs.parser.options/filetype) |  |
| size | long |  |
| encrypted | boolean |  |

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Получает тип документа.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getSize() {#getSize--}
```
public long getSize()
```


Получает размер документа в байтах.


**Returns:**
long - Целочисленное значение, представляющее размер документа в байтах.

### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


Получает значение, представляющее, защищён ли файл паролем.


**Returns:**
boolean - Значение true, если файл защищён паролем; иначе false.


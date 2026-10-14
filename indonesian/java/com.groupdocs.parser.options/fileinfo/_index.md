---
title: "FileInfo"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili informasi file."
type: docs
weight: 19
url: /id/java/com.groupdocs.parser.options/fileinfo/
---
**Inheritance:**
java.lang.Object
```
public class FileInfo
```

Mewakili informasi file.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [FileInfo(FileType fileType, long size, boolean encrypted)](#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getFileType()](#getFileType--) | Mendapatkan tipe dokumen. |
|
|  | [getSize()](#getSize--) | Mendapatkan ukuran dokumen dalam byte. |
|
|  | [isEncrypted()](#isEncrypted--) | Mendapatkan nilai yang menunjukkan apakah file dilindungi kata sandi. |
|
### FileInfo(FileType fileType, long size, boolean encrypted) {#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-}
```
public FileInfo(FileType fileType, long size, boolean encrypted)
```


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileType | [FileType](../../com.groupdocs.parser.options/filetype) |  |
| size | long |  |
| encrypted | boolean |  |

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Mendapatkan tipe dokumen.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getSize() {#getSize--}
```
public long getSize()
```


Mendapatkan ukuran dokumen dalam byte.


**Returns:**
long - Nilai integer yang mewakili ukuran dokumen dalam byte.

### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


Mendapatkan nilai yang menunjukkan apakah file dilindungi kata sandi.


**Returns:**
boolean - true boolean jika file dilindungi kata sandi; jika tidak false.


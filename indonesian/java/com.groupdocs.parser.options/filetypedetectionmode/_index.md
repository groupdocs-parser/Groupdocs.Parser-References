---
title: "FileTypeDetectionMode"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mendefinisikan mode deteksi tipe file."
type: docs
weight: 44
url: /id/java/com.groupdocs.parser.options/filetypedetectionmode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum FileTypeDetectionMode extends Enum<FileTypeDetectionMode>
```

Mendefinisikan mode deteksi tipe file.

## Bidang

| Bidang | Deskripsi |
| --- | --- |
|  | [Default](#Default) | Tipe file dideteksi berdasarkan ekstensi file; jika ekstensi file tidak dikenali, tipe file dideteksi berdasarkan konten file. |
|
|  | [Extension](#Extension) | Tipe file hanya dideteksi berdasarkan ekstensi file. |
|
|  | [Content](#Content) | Tipe file hanya dideteksi berdasarkan konten file. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Default {#Default}
```
public static final FileTypeDetectionMode Default
```


Tipe file dideteksi berdasarkan ekstensi file; jika ekstensi file tidak dikenali, tipe file dideteksi berdasarkan konten file.


### Extension {#Extension}
```
public static final FileTypeDetectionMode Extension
```


Tipe file hanya dideteksi berdasarkan ekstensi file.


### Content {#Content}
```
public static final FileTypeDetectionMode Content
```


Tipe file hanya dideteksi berdasarkan konten file.


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
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | java.lang.String |  |

**Returns:**
[FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode)

---
title: "FileInfo"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Dateiinformationen dar."
type: docs
weight: 19
url: /de/java/com.groupdocs.parser.options/fileinfo/
---
**Inheritance:**
java.lang.Object
```
public class FileInfo
```

Stellt die Dateiinformationen dar.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [FileInfo(FileType fileType, long size, boolean encrypted)](#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getFileType()](#getFileType--) | Liefert den Dokumenttyp. |
|
|  | [getSize()](#getSize--) | Liefert die Größe des Dokuments in Bytes. |
|
|  | [isEncrypted()](#isEncrypted--) | Liefert einen Wert, der angibt, ob eine Datei passwortgeschützt ist. |
|
### FileInfo(FileType fileType, long size, boolean encrypted) {#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-}
```
public FileInfo(FileType fileType, long size, boolean encrypted)
```


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileType | [FileType](../../com.groupdocs.parser.options/filetype) |  |
| size | long |  |
| encrypted | boolean |  |

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Liefert den Dokumenttyp.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getSize() {#getSize--}
```
public long getSize()
```


Liefert die Größe des Dokuments in Bytes.


**Returns:**
long - Ein ganzzahliger Wert, der die Größe des Dokuments in Bytes darstellt.

### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


Liefert einen Wert, der angibt, ob eine Datei passwortgeschützt ist.


**Returns:**
boolean - Ein boolescher Wert true, wenn eine Datei passwortgeschützt ist; andernfalls false.


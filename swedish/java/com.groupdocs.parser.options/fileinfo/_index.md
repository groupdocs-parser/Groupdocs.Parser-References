---
title: "FileInfo"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar filinformationen."
type: docs
weight: 19
url: /sv/java/com.groupdocs.parser.options/fileinfo/
---
**Inheritance:**
java.lang.Object
```
public class FileInfo
```

Representerar filinformationen.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [FileInfo(FileType fileType, long size, boolean encrypted)](#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getFileType()](#getFileType--) | Hämtar dokumenttypen. |
|
|  | [getSize()](#getSize--) | Hämtar storleken på dokumentet i byte. |
|
|  | [isEncrypted()](#isEncrypted--) | Hämtar ett värde som representerar om en fil är lösenordsskyddad. |
|
### FileInfo(FileType fileType, long size, boolean encrypted) {#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-}
```
public FileInfo(FileType fileType, long size, boolean encrypted)
```


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileType | [FileType](../../com.groupdocs.parser.options/filetype) |  |
| size | long |  |
| encrypted | boolean |  |

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Hämtar dokumenttypen.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getSize() {#getSize--}
```
public long getSize()
```


Hämtar storleken på dokumentet i byte.


**Returns:**
long - Ett heltal som representerar storleken på dokumentet i byte.

### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


Hämtar ett värde som representerar om en fil är lösenordsskyddad.


**Returns:**
boolean - En boolean true om en fil är lösenordsskyddad; annars false.


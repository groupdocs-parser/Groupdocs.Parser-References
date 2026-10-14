---
title: "FileInfo"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt de bestandsinformatie voor."
type: docs
weight: 19
url: /nl/java/com.groupdocs.parser.options/fileinfo/
---
**Inheritance:**
java.lang.Object
```
public class FileInfo
```

Stelt de bestandsinformatie voor.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [FileInfo(FileType fileType, long size, boolean encrypted)](#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getFileType()](#getFileType--) | Haalt het documenttype op. |
|
|  | [getSize()](#getSize--) | Haalt de grootte van het document op in bytes. |
|
|  | [isEncrypted()](#isEncrypted--) | Haalt een waarde op die aangeeft of een bestand met een wachtwoord is beveiligd. |
|
### FileInfo(FileType fileType, long size, boolean encrypted) {#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-}
```
public FileInfo(FileType fileType, long size, boolean encrypted)
```


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileType | [FileType](../../com.groupdocs.parser.options/filetype) |  |
| size | long |  |
| encrypted | boolean |  |

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Haalt het documenttype op.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getSize() {#getSize--}
```
public long getSize()
```


Haalt de grootte van het document op in bytes.


**Returns:**
long - Een gehele waarde die de grootte van het document in bytes vertegenwoordigt.

### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


Haalt een waarde op die aangeeft of een bestand met een wachtwoord is beveiligd.


**Returns:**
boolean - Een boolean true als een bestand met een wachtwoord is beveiligd; anders false.


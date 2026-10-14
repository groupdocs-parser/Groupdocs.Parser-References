---
title: "FileInfo"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente les informations du fichier."
type: docs
weight: 19
url: /fr/java/com.groupdocs.parser.options/fileinfo/
---
**Inheritance:**
java.lang.Object
```
public class FileInfo
```

Représente les informations du fichier.

## Constructors

| Constructor | Description |
| --- | --- |
| [FileInfo(FileType fileType, long size, boolean encrypted)](#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-) |  |
## Methods

| Method | Description |
| --- | --- |
|  | [getFileType()](#getFileType--) | Obtient le type de document. |
|
|  | [getSize()](#getSize--) | Obtient la taille du document en octets. |
|
|  | [isEncrypted()](#isEncrypted--) | Obtient une valeur qui indique si un fichier est protégé par mot de passe. |
|
### FileInfo(FileType fileType, long size, boolean encrypted) {#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-}
```
public FileInfo(FileType fileType, long size, boolean encrypted)
```


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileType | [FileType](../../com.groupdocs.parser.options/filetype) |  |
| size | long |  |
| crypté | boolean |  |

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Obtient le type de document.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getSize() {#getSize--}
```
public long getSize()
```


Obtient la taille du document en octets.


**Returns:**
long - Une valeur entière qui représente la taille du document en octets.

### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


Obtient une valeur qui indique si un fichier est protégé par mot de passe.


**Returns:**
boolean - Un booléen vrai si un fichier est protégé par mot de passe ; sinon faux.


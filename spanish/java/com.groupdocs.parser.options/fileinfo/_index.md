---
title: "FileInfo"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa la información del archivo."
type: docs
weight: 19
url: /es/java/com.groupdocs.parser.options/fileinfo/
---
**Inheritance:**
java.lang.Object
```
public class FileInfo
```

Representa la información del archivo.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [FileInfo(FileType fileType, long size, boolean encrypted)](#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getFileType()](#getFileType--) | Obtiene el tipo de documento. |
|
|  | [getSize()](#getSize--) | Obtiene el tamaño del documento en bytes. |
|
|  | [isEncrypted()](#isEncrypted--) | Obtiene un valor que indica si un archivo está protegido con contraseña. |
|
### FileInfo(FileType fileType, long size, boolean encrypted) {#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-}
```
public FileInfo(FileType fileType, long size, boolean encrypted)
```


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileType | [FileType](../../com.groupdocs.parser.options/filetype) |  |
| size | long |  |
| encrypted | boolean |  |

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Obtiene el tipo de documento.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getSize() {#getSize--}
```
public long getSize()
```


Obtiene el tamaño del documento en bytes.


**Returns:**
long - Un valor entero que representa el tamaño del documento en bytes.

### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


Obtiene un valor que indica si un archivo está protegido con contraseña.


**Returns:**
boolean - Un booleano true si un archivo está protegido con contraseña; de lo contrario false.


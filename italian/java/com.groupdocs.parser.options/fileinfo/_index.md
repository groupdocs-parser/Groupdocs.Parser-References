---
title: "FileInfo"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta le informazioni del file."
type: docs
weight: 19
url: /it/java/com.groupdocs.parser.options/fileinfo/
---
**Inheritance:**
java.lang.Object
```
public class FileInfo
```

Rappresenta le informazioni del file.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [FileInfo(FileType fileType, long size, boolean encrypted)](#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getFileType()](#getFileType--) | Restituisce il tipo di documento. |
|
|  | [getSize()](#getSize--) | Restituisce la dimensione del documento in byte. |
|
|  | [isEncrypted()](#isEncrypted--) | Restituisce un valore che indica se un file è protetto da password. |
|
### FileInfo(FileType fileType, long size, boolean encrypted) {#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-}
```
public FileInfo(FileType fileType, long size, boolean encrypted)
```


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileType | [FileType](../../com.groupdocs.parser.options/filetype) |  |
| size | long |  |
| encrypted | boolean |  |

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Restituisce il tipo di documento.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getSize() {#getSize--}
```
public long getSize()
```


Restituisce la dimensione del documento in byte.


**Returns:**
long - Un valore intero che rappresenta la dimensione del documento in byte.

### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


Restituisce un valore che indica se un file è protetto da password.


**Returns:**
boolean - Un valore booleano true se un file è protetto da password; altrimenti false.


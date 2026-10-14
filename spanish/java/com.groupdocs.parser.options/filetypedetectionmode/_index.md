---
title: "FileTypeDetectionMode"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Define un modo de detección del tipo de archivo."
type: docs
weight: 44
url: /es/java/com.groupdocs.parser.options/filetypedetectionmode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum FileTypeDetectionMode extends Enum<FileTypeDetectionMode>
```

Define un modo de detección del tipo de archivo.

## Campos

| Campo | Descripción |
| --- | --- |
|  | [Default](#Default) | El tipo de archivo se detecta por la extensión del archivo; si la extensión del archivo no se reconoce, el tipo de archivo se detecta por el contenido del archivo. |
|
|  | [Extension](#Extension) | El tipo de archivo se detecta solo por la extensión del archivo. |
|
|  | [Content](#Content) | El tipo de archivo se detecta solo por el contenido del archivo. |
|
## Métodos

| Método | Descripción |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Default {#Default}
```
public static final FileTypeDetectionMode Default
```


El tipo de archivo se detecta por la extensión del archivo; si la extensión del archivo no se reconoce, el tipo de archivo se detecta por el contenido del archivo.


### Extension {#Extension}
```
public static final FileTypeDetectionMode Extension
```


El tipo de archivo se detecta solo por la extensión del archivo.


### Content {#Content}
```
public static final FileTypeDetectionMode Content
```


El tipo de archivo se detecta solo por el contenido del archivo.


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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String |  |

**Returns:**
[FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode)

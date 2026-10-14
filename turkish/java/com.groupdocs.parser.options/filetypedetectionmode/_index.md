---
title: "FileTypeDetectionMode"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Dosya türü algılamanın bir modunu tanımlar."
type: docs
weight: 44
url: /tr/java/com.groupdocs.parser.options/filetypedetectionmode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum FileTypeDetectionMode extends Enum<FileTypeDetectionMode>
```

Dosya türü algılamanın bir modunu tanımlar.

## Alanlar

| Alan | Açıklama |
| --- | --- |
|  | [Default](#Default) | Dosya türü dosya uzantısına göre algılanır; dosya uzantısı tanınmazsa, dosya türü dosya içeriğine göre algılanır. |
|
|  | [Extension](#Extension) | Dosya türü yalnızca dosya uzantısına göre algılanır. |
|
|  | [Content](#Content) | Dosya türü yalnızca dosya içeriğine göre algılanır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Default {#Default}
```
public static final FileTypeDetectionMode Default
```


Dosya türü dosya uzantısına göre algılanır; dosya uzantısı tanınmazsa, dosya türü dosya içeriğine göre algılanır.


### Extension {#Extension}
```
public static final FileTypeDetectionMode Extension
```


Dosya türü yalnızca dosya uzantısına göre algılanır.


### Content {#Content}
```
public static final FileTypeDetectionMode Content
```


Dosya türü yalnızca dosya içeriğine göre algılanır.


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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String |  |

**Returns:**
[FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode)

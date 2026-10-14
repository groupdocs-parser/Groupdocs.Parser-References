---
title: "FileTypeDetectionMode"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Definierar ett läge för filtypdetektering."
type: docs
weight: 44
url: /sv/java/com.groupdocs.parser.options/filetypedetectionmode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum FileTypeDetectionMode extends Enum<FileTypeDetectionMode>
```

Definierar ett läge för filtypdetektering.

## Fält

| Fält | Beskrivning |
| --- | --- |
|  | [Default](#Default) | Filtypen upptäcks via filändelsen; om filändelsen inte känns igen, upptäcks filtypen via filinnehållet. |
|
|  | [Extension](#Extension) | Filtypen upptäcks endast av filändelsen. |
|
|  | [Content](#Content) | Filtypen upptäcks endast av filinnehållet. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Default {#Default}
```
public static final FileTypeDetectionMode Default
```


Filtypen upptäcks via filändelsen; om filändelsen inte känns igen, upptäcks filtypen via filinnehållet.


### Extension {#Extension}
```
public static final FileTypeDetectionMode Extension
```


Filtypen upptäcks endast av filändelsen.


### Content {#Content}
```
public static final FileTypeDetectionMode Content
```


Filtypen upptäcks endast av filinnehållet.


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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | java.lang.String |  |

**Returns:**
[FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode)

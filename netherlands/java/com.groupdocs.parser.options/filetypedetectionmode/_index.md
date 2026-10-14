---
title: "FileTypeDetectionMode"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Definieert een modus van de bestandstype-detectie."
type: docs
weight: 44
url: /nl/java/com.groupdocs.parser.options/filetypedetectionmode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum FileTypeDetectionMode extends Enum<FileTypeDetectionMode>
```

Definieert een modus van de bestandstype-detectie.

## Velden

| Veld | Beschrijving |
| --- | --- |
|  | [Default](#Default) | Het bestandstype wordt gedetecteerd op basis van de bestandsextensie; als de extensie niet wordt herkend, wordt het bestandstype gedetecteerd op basis van de bestandsinhoud. |
|
|  | [Extension](#Extension) | Het bestandstype wordt alleen gedetecteerd op basis van de bestandsextensie. |
|
|  | [Content](#Content) | Het bestandstype wordt alleen gedetecteerd op basis van de bestandsinhoud. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Default {#Default}
```
public static final FileTypeDetectionMode Default
```


Het bestandstype wordt gedetecteerd op basis van de bestandsextensie; als de extensie niet wordt herkend, wordt het bestandstype gedetecteerd op basis van de bestandsinhoud.


### Extension {#Extension}
```
public static final FileTypeDetectionMode Extension
```


Het bestandstype wordt alleen gedetecteerd op basis van de bestandsextensie.


### Content {#Content}
```
public static final FileTypeDetectionMode Content
```


Het bestandstype wordt alleen gedetecteerd op basis van de bestandsinhoud.


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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String |  |

**Returns:**
[FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode)

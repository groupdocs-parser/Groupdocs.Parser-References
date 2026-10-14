---
title: "FileTypeDetectionMode"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Definiert einen Modus der Dateityp-Erkennung."
type: docs
weight: 44
url: /de/java/com.groupdocs.parser.options/filetypedetectionmode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum FileTypeDetectionMode extends Enum<FileTypeDetectionMode>
```

Definiert einen Modus der Dateityp-Erkennung.

## Felder

| Feld | Beschreibung |
| --- | --- |
|  | [Default](#Default) | Der Dateityp wird anhand der Dateierweiterung erkannt; wenn die Dateierweiterung nicht erkannt wird, wird der Dateityp anhand des Dateiinhalts ermittelt. |
|
|  | [Extension](#Extension) | Der Dateityp wird ausschließlich anhand der Dateierweiterung erkannt. |
|
|  | [Content](#Content) | Der Dateityp wird ausschließlich anhand des Dateiinhalts erkannt. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Default {#Default}
```
public static final FileTypeDetectionMode Default
```


Der Dateityp wird anhand der Dateierweiterung erkannt; wenn die Dateierweiterung nicht erkannt wird, wird der Dateityp anhand des Dateiinhalts ermittelt.


### Extension {#Extension}
```
public static final FileTypeDetectionMode Extension
```


Der Dateityp wird ausschließlich anhand der Dateierweiterung erkannt.


### Content {#Content}
```
public static final FileTypeDetectionMode Content
```


Der Dateityp wird ausschließlich anhand des Dateiinhalts erkannt.


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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |

**Returns:**
[FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode)

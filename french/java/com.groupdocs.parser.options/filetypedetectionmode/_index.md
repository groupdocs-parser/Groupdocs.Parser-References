---
title: "FileTypeDetectionMode"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Définit un mode de détection du type de fichier."
type: docs
weight: 44
url: /fr/java/com.groupdocs.parser.options/filetypedetectionmode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum FileTypeDetectionMode extends Enum<FileTypeDetectionMode>
```

Définit un mode de détection du type de fichier.

## Champs

| Champ | Description |
| --- | --- |
|  | [Default](#Default) | Le type de fichier est détecté par l'extension du fichier ; si l'extension du fichier n'est pas reconnue, le type de fichier est détecté par le contenu du fichier. |
|
|  | [Extension](#Extension) | Le type de fichier est détecté uniquement par l'extension du fichier. |
|
|  | [Content](#Content) | Le type de fichier est détecté uniquement par le contenu du fichier. |
|
## Methods

| Method | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Default {#Default}
```
public static final FileTypeDetectionMode Default
```


Le type de fichier est détecté par l'extension du fichier ; si l'extension du fichier n'est pas reconnue, le type de fichier est détecté par le contenu du fichier.


### Extension {#Extension}
```
public static final FileTypeDetectionMode Extension
```


Le type de fichier est détecté uniquement par l'extension du fichier.


### Content {#Content}
```
public static final FileTypeDetectionMode Content
```


Le type de fichier est détecté uniquement par le contenu du fichier.


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
| Parameter | Type | Description |
| --- | --- | --- |
| nom | java.lang.String |  |

**Returns:**
[FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode)

---
title: "FileTypeDetectionMode"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Definisce una modalità di rilevamento del tipo di file."
type: docs
weight: 44
url: /it/java/com.groupdocs.parser.options/filetypedetectionmode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum FileTypeDetectionMode extends Enum<FileTypeDetectionMode>
```

Definisce una modalità di rilevamento del tipo di file.

## Fields

| Field | Descrizione |
| --- | --- |
|  | [Default](#Default) | Il tipo di file viene rilevato dall'estensione del file; se l'estensione del file non è riconosciuta, il tipo di file viene rilevato dal contenuto del file. |
|
|  | [Extension](#Extension) | Il tipo di file viene rilevato solo dall'estensione del file. |
|
|  | [Content](#Content) | Il tipo di file viene rilevato solo dal contenuto del file. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Default {#Default}
```
public static final FileTypeDetectionMode Default
```


Il tipo di file viene rilevato dall'estensione del file; se l'estensione del file non è riconosciuta, il tipo di file viene rilevato dal contenuto del file.


### Extension {#Extension}
```
public static final FileTypeDetectionMode Extension
```


Il tipo di file viene rilevato solo dall'estensione del file.


### Content {#Content}
```
public static final FileTypeDetectionMode Content
```


Il tipo di file viene rilevato solo dal contenuto del file.


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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode)

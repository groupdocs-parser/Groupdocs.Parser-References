---
title: "QualityMode"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Définit un niveau de qualité."
type: docs
weight: 48
url: /fr/java/com.groupdocs.parser.options/qualitymode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum QualityMode extends Enum<QualityMode>
```

Définit un niveau de qualité.

## Champs

| Champ | Description |
| --- | --- |
|  | [High](#High) | Haute qualité. |
|
|  | [Normal](#Normal) | Qualité normale. |
|
|  | [Low](#Low) | Basse qualité. |
|
## Methods

| Method | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### High {#High}
```
public static final QualityMode High
```


Haute qualité. Des algorithmes de traitement rapides sont utilisés.


### Normal {#Normal}
```
public static final QualityMode Normal
```


Qualité normale. Des algorithmes de traitement par défaut sont utilisés.


### Low {#Low}
```
public static final QualityMode Low
```


Basse qualité. Des algorithmes de traitement lents sont utilisés.


### values() {#values--}
```
public static QualityMode[] values()
```




**Returns:**
com.groupdocs.parser.options.QualityMode[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static QualityMode valueOf(String name)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| nom | java.lang.String |  |

**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode)

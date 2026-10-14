---
title: "QualityMode"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Definiert ein Qualitätsniveau."
type: docs
weight: 48
url: /de/java/com.groupdocs.parser.options/qualitymode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum QualityMode extends Enum<QualityMode>
```

Definiert ein Qualitätsniveau.

## Felder

| Feld | Beschreibung |
| --- | --- |
|  | [High](#High) | Hohe Qualität. |
|
|  | [Normal](#Normal) | Normale Qualität. |
|
|  | [Low](#Low) | Niedrige Qualität. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### High {#High}
```
public static final QualityMode High
```


Hohe Qualität. Schnelle Verarbeitungsalgorithmen werden verwendet.


### Normal {#Normal}
```
public static final QualityMode Normal
```


Normale Qualität. Standard-Verarbeitungsalgorithmen werden verwendet.


### Low {#Low}
```
public static final QualityMode Low
```


Niedrige Qualität. Langsame Verarbeitungsalgorithmen werden verwendet.


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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |

**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode)

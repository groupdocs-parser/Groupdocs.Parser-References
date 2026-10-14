---
title: "QualityMode"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Definierar en kvalitetsnivå."
type: docs
weight: 48
url: /sv/java/com.groupdocs.parser.options/qualitymode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum QualityMode extends Enum<QualityMode>
```

Definierar en kvalitetsnivå.

## Fält

| Fält | Beskrivning |
| --- | --- |
|  | [High](#High) | Hög kvalitet. |
|
|  | [Normal](#Normal) | Normal kvalitet. |
|
|  | [Low](#Low) | Låg kvalitet. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### High {#High}
```
public static final QualityMode High
```


Hög kvalitet. Snabba bearbetningsalgoritmer används.


### Normal {#Normal}
```
public static final QualityMode Normal
```


Normal kvalitet. Standardbearbetningsalgoritmer används.


### Low {#Low}
```
public static final QualityMode Low
```


Låg kvalitet. Långsamma bearbetningsalgoritmer används.


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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | java.lang.String |  |

**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode)

---
title: "QualityMode"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Definisce un livello di qualità."
type: docs
weight: 48
url: /it/java/com.groupdocs.parser.options/qualitymode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum QualityMode extends Enum<QualityMode>
```

Definisce un livello di qualità.

## Fields

| Field | Descrizione |
| --- | --- |
|  | [High](#High) | Qualità alta. |
|
|  | [Normal](#Normal) | Qualità normale. |
|
|  | [Low](#Low) | Qualità bassa. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### High {#High}
```
public static final QualityMode High
```


Qualità alta. Vengono utilizzati algoritmi di elaborazione rapidi.


### Normal {#Normal}
```
public static final QualityMode Normal
```


Qualità normale. Vengono utilizzati gli algoritmi di elaborazione predefiniti.


### Low {#Low}
```
public static final QualityMode Low
```


Qualità bassa. Vengono utilizzati algoritmi di elaborazione lenti.


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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode)

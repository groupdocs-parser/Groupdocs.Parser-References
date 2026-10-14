---
title: "QualityMode"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Definieert een kwaliteitsniveau."
type: docs
weight: 48
url: /nl/java/com.groupdocs.parser.options/qualitymode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum QualityMode extends Enum<QualityMode>
```

Definieert een kwaliteitsniveau.

## Velden

| Veld | Beschrijving |
| --- | --- |
|  | [High](#High) | Hoge kwaliteit. |
|
|  | [Normal](#Normal) | Normale kwaliteit. |
|
|  | [Low](#Low) | Lage kwaliteit. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### High {#High}
```
public static final QualityMode High
```


Hoge kwaliteit. Snelle verwerkingsalgoritmen worden gebruikt.


### Normal {#Normal}
```
public static final QualityMode Normal
```


Normale kwaliteit. Standaard verwerkingsalgoritmen worden gebruikt.


### Low {#Low}
```
public static final QualityMode Low
```


Lage kwaliteit. Trage verwerkingsalgoritmen worden gebruikt.


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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String |  |

**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode)

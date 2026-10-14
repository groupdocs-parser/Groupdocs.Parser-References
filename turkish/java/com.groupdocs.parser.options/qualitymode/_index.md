---
title: "QualityMode"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Kalite seviyesini tanımlar."
type: docs
weight: 48
url: /tr/java/com.groupdocs.parser.options/qualitymode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum QualityMode extends Enum<QualityMode>
```

Kalite seviyesini tanımlar.

## Alanlar

| Alan | Açıklama |
| --- | --- |
|  | [High](#High) | Yüksek kalite. |
|
|  | [Normal](#Normal) | Normal kalite. |
|
|  | [Low](#Low) | Düşük kalite. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### High {#High}
```
public static final QualityMode High
```


Yüksek kalite. Hızlı işleme algoritmaları kullanılır.


### Normal {#Normal}
```
public static final QualityMode Normal
```


Normal kalite. Varsayılan işleme algoritmaları kullanılır.


### Low {#Low}
```
public static final QualityMode Low
```


Düşük kalite. Yavaş işleme algoritmaları kullanılır.


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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String |  |

**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode)

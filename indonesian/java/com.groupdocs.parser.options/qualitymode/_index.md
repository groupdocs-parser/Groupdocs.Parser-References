---
title: "QualityMode"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mendefinisikan tingkat kualitas."
type: docs
weight: 48
url: /id/java/com.groupdocs.parser.options/qualitymode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum QualityMode extends Enum<QualityMode>
```

Mendefinisikan tingkat kualitas.

## Bidang

| Bidang | Deskripsi |
| --- | --- |
|  | [High](#High) | Kualitas tinggi. |
|
|  | [Normal](#Normal) | Kualitas normal. |
|
|  | [Low](#Low) | Kualitas rendah. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### High {#High}
```
public static final QualityMode High
```


Kualitas tinggi. Algoritma pemrosesan cepat digunakan.


### Normal {#Normal}
```
public static final QualityMode Normal
```


Kualitas normal. Algoritma pemrosesan default digunakan.


### Low {#Low}
```
public static final QualityMode Low
```


Kualitas rendah. Algoritma pemrosesan lambat digunakan.


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
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | java.lang.String |  |

**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode)

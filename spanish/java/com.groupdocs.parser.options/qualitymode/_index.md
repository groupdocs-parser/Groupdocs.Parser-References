---
title: "QualityMode"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Define un nivel de calidad."
type: docs
weight: 48
url: /es/java/com.groupdocs.parser.options/qualitymode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum QualityMode extends Enum<QualityMode>
```

Define un nivel de calidad.

## Campos

| Campo | Descripción |
| --- | --- |
|  | [High](#High) | Alta calidad. |
|
|  | [Normal](#Normal) | Calidad normal. |
|
|  | [Low](#Low) | Baja calidad. |
|
## Métodos

| Método | Descripción |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### High {#High}
```
public static final QualityMode High
```


Alta calidad. Se utilizan algoritmos de procesamiento rápidos.


### Normal {#Normal}
```
public static final QualityMode Normal
```


Calidad normal. Se utilizan algoritmos de procesamiento predeterminados.


### Low {#Low}
```
public static final QualityMode Low
```


Baja calidad. Se utilizan algoritmos de procesamiento lentos.


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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String |  |

**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode)

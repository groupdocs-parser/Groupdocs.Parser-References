---
title: "QualityMode"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Определяет уровень качества."
type: docs
weight: 48
url: /ru/java/com.groupdocs.parser.options/qualitymode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum QualityMode extends Enum<QualityMode>
```

Определяет уровень качества.

## Поля

| Поле | Описание |
| --- | --- |
|  | [High](#High) | Высокое качество. |
|
|  | [Normal](#Normal) | Нормальное качество. |
|
|  | [Low](#Low) | Низкое качество. |
|
## Методы

| Метод | Описание |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### High {#High}
```
public static final QualityMode High
```


Высокое качество. Используются быстрые алгоритмы обработки.


### Normal {#Normal}
```
public static final QualityMode Normal
```


Нормальное качество. Используются алгоритмы обработки по умолчанию.


### Low {#Low}
```
public static final QualityMode Low
```


Низкое качество. Используются медленные алгоритмы обработки.


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
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String |  |

**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode)

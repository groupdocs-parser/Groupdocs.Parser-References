---
title: "TemplatePosition"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет базовый абстрактный класс для позиций шаблона."
type: docs
weight: 18
url: /ru/java/com.groupdocs.parser.templates/templateposition/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplatePosition
```

Предоставляет базовый абстрактный класс для позиций шаблона.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [TemplatePosition()](#TemplatePosition--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | Создаёт копию текущей позиции со всеми координатами, масштабированными на заданный коэффициент. |
|
### TemplatePosition() {#TemplatePosition--}
```
public TemplatePosition()
```


### scale(double factor) {#scale-double-}
```
public abstract TemplatePosition scale(double factor)
```


Создаёт копию текущей позиции со всеми координатами, масштабированными на заданный коэффициент.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | коэффициент | double | Коэффициент масштабирования. |
|

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - A new [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) with scaled coordinates.


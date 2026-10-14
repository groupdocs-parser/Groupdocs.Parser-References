---
title: "TemplateItem"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет базовый абстрактный класс для элементов шаблона."
type: docs
weight: 14
url: /ru/java/com.groupdocs.parser.templates/templateitem/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplateItem
```

Предоставляет базовый абстрактный класс для элементов шаблона.

Наследники класса [TemplateItem](../../com.groupdocs.parser.templates/templateitem) используются в коллекции [Template](../../com.groupdocs.parser.templates/template).

## Методы

| Метод | Описание |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | Создаёт копию текущего элемента, масштабируя все координаты на заданный коэффициент. |
|
|  | [getName()](#getName--) | Получает имя элемента шаблона. |
|
|  | [getPageIndex()](#getPageIndex--) | Получает индекс страницы элемента шаблона. |
|
|  | [getPageWidth()](#getPageWidth--) | Получает ширину страницы, использованной для создания элемента шаблона. |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | Получает значение, указывающее, было ли  Name  преобразовано в ВЕРХНИЙ РЕГИСТР. |
|
### scale(double factor) {#scale-double-}
```
public abstract TemplateItem scale(double factor)
```


Создаёт копию текущего элемента, масштабируя все координаты на заданный коэффициент.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | коэффициент | double | Коэффициент масштабирования. |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - A new [TemplateItem](../../com.groupdocs.parser.templates/templateitem) with scaled coordinates.

### getName() {#getName--}
```
public String getName()
```


Получает имя элемента шаблона.


**Returns:**
java.lang.String - Строковое значение в верхнем регистре, представляющее имя элемента шаблона.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Получает индекс страницы элемента шаблона.


**Returns:**
java.lang.Integer - Целочисленное значение, представляющее индекс страницы, на которой расположен элемент шаблона;  null  если элемент шаблона расположен на любой странице.

### getPageWidth() {#getPageWidth--}
```
public Double getPageWidth()
```


Получает ширину страницы, использованной для создания элемента шаблона.


**Returns:**
java.lang.Double - Ширина страницы в пикселях;  null  если ширина страницы неизвестна.

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


Получает значение, указывающее, было ли  Name  преобразовано в ВЕРХНИЙ РЕГИСТР.


**Returns:**
boolean - Булево значение, указывающее, было ли  Name  преобразовано в ВЕРХНИЙ РЕГИСТР.


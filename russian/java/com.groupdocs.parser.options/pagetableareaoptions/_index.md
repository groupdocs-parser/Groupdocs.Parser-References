---
title: "PageTableAreaOptions"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет параметры, используемые для извлечения областей таблиц страниц."
type: docs
weight: 31
url: /ru/java/com.groupdocs.parser.options/pagetableareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTableAreaOptions extends PageAreaOptions
```

Предоставляет параметры, используемые для извлечения областей таблиц страниц.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [PageTableAreaOptions(TemplateTableLayout tableLayout)](#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-) | Инициализирует новый экземпляр класса [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions). |
|
|  | [PageTableAreaOptions(Rectangle rectangle)](#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-) | Инициализирует новый экземпляр класса [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) с прямоугольником поиска и без фиксированного макета. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getTableLayout()](#getTableLayout--) | Получает макет таблицы, определяющий таблицу на странице. |
|
### PageTableAreaOptions(TemplateTableLayout tableLayout) {#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-}
```
public PageTableAreaOptions(TemplateTableLayout tableLayout)
```


Инициализирует новый экземпляр класса [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | tableLayout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Макет таблицы, определяющий таблицу на странице. |
|

### PageTableAreaOptions(Rectangle rectangle) {#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageTableAreaOptions(Rectangle rectangle)
```


Инициализирует новый экземпляр класса [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) с прямоугольником поиска и без фиксированного макета.

Полезно для ограничения автоматически обнаруженных таблиц областью страницы. Отражает C#

new PageTableAreaOptions(null) { Rectangle = ... }
шаблон.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область на странице, где следует обнаруживать таблицы; передайте  null  для поиска по всей странице. |
|

### getTableLayout() {#getTableLayout--}
```
public TemplateTableLayout getTableLayout()
```


Получает макет таблицы, определяющий таблицу на странице.


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instane of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class.


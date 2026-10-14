---
title: "PageGroupArea"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет группу областей страницы, которая используется для группировки разных типов блоков страницы документа в функции разбора по шаблону."
type: docs
weight: 19
url: /ru/java/com.groupdocs.parser.data/pagegrouparea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageGroupArea extends PageArea
```

Представляет группу областей страницы, которая используется для группировки разных типов блоков страницы документа в функции разбора по шаблону.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [PageGroupArea(Iterable<PageArea> areas, Page page)](#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-) | Создаёт новый экземпляр класса [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getAreas()](#getAreas--) | Возвращает коллекцию сгруппированных областей страниц. |
|
### PageGroupArea(Iterable<PageArea> areas, Page page) {#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-}
```
public PageGroupArea(Iterable<PageArea> areas, Page page)
```


Создаёт новый экземпляр класса [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | areas | java.lang.Iterable<com.groupdocs.parser.data.PageArea> | Коллекция областей страниц, которые будут сгруппированы. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Страница, содержащая область. |
|

### getAreas() {#getAreas--}
```
public Iterable<PageArea> getAreas()
```


Возвращает коллекцию сгруппированных областей страниц.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageArea> - Коллекция объектов [PageArea](../../com.groupdocs.parser.data/pagearea).


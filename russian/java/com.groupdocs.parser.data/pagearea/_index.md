---
title: "PageArea"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет абстрактный базовый класс для областей страницы, которые используются для представления блоков на странице документа в функции разбора по шаблону."
type: docs
weight: 17
url: /ru/java/com.groupdocs.parser.data/pagearea/
---
**Inheritance:**
java.lang.Object
```
public abstract class PageArea
```

Представляет абстрактный базовый класс для областей страницы, которые используются для представления блоков на странице документа в функции разбора по шаблону.

## Методы

| Метод | Описание |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Возвращает прямоугольную область. |
|
|  | [getPage()](#getPage--) | Возвращает информацию о странице документа, такую как индекс страницы и размер страницы. |
|
### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Возвращает прямоугольную область.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area of the page that contains the page area.

### getPage() {#getPage--}
```
public Page getPage()
```


Возвращает информацию о странице документа, такую как индекс страницы и размер страницы.


**Returns:**
[Page](../../com.groupdocs.parser.data/page) - An instance of [Page](../../com.groupdocs.parser.data/page) class that represents the page that contains the page area.


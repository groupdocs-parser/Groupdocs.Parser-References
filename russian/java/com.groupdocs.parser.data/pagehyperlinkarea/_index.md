---
title: "PageHyperlinkArea"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет область страницы, которая используется для представления гиперссылки на странице."
type: docs
weight: 20
url: /ru/java/com.groupdocs.parser.data/pagehyperlinkarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageHyperlinkArea extends PageArea
```

Представляет область страницы, которая используется для представления гиперссылки на странице.

Экземпляр класса [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) используется в качестве возвращаемого значения следующих методов:

* [Parser.getHyperlinks()](../../com.groupdocs.parser/parser#getHyperlinks--)
* [Parser.getHyperlinks(PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-PageAreaOptions-)
* [Parser.getHyperlinks(int)](../../com.groupdocs.parser/parser#getHyperlinks-int-)
* [Parser.getHyperlinks(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-int--PageAreaOptions-)

Смотрите примеры использования там.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)](#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Инициализирует новый экземпляр класса [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getText()](#getText--) | Получает текст гиперссылки. |
|
|  | [getUrl()](#getUrl--) | Получает URL гиперссылки. |
|
### PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle) {#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)
```


Инициализирует новый экземпляр класса [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | текст | java.lang.String | Текст гиперссылки. |
|
|  | url | java.lang.String | URL гиперссылки. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Страница, содержащая гиперссылку. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область, содержащая гиперссылку. |
|

### getText() {#getText--}
```
public String getText()
```


Получает текст гиперссылки.


**Returns:**
java.lang.String - Строковое значение, представляющее текст гиперссылки.

### getUrl() {#getUrl--}
```
public String getUrl()
```


Получает URL гиперссылки.


**Returns:**
java.lang.String - Строковое значение, представляющее URL гиперссылки.


---
title: "HighlightItem"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет выделение части текста, которое обычно используется для объяснения контекста найденного текста в функции поиска."
type: docs
weight: 14
url: /ru/java/com.groupdocs.parser.data/highlightitem/
---
**Inheritance:**
java.lang.Object
```
public class HighlightItem
```

Представляет выделение, часть текста, обычно используемую для объяснения контекста найденного текста в функции поиска.

Экземпляр класса [HighlightItem](../../com.groupdocs.parser.data/highlightitem) используется в качестве возвращаемого значения метода [Parser.getHighlight(int, boolean, com.groupdocs.parser.options.HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--com.groupdocs.parser.options.HighlightOptions-).
[SearchResult.getLeftHighlightItem()](../../com.groupdocs.parser.data/searchresult#getLeftHighlightItem--) and [SearchResult.getRightHighlightItem()](../../com.groupdocs.parser.data/searchresult#getRightHighlightItem--) properties. See the usage examples there.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [HighlightItem(int position, String text)](#HighlightItem-int-java.lang.String-) | Инициализирует новый экземпляр класса [HighlightItem](../../com.groupdocs.parser.data/highlightitem). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getPosition()](#getPosition--) | Получает позицию в тексте документа. |
|
|  | [getText()](#getText--) | Получает текст выделения. |
|
### HighlightItem(int position, String text) {#HighlightItem-int-java.lang.String-}
```
public HighlightItem(int position, String text)
```


Инициализирует новый экземпляр класса [HighlightItem](../../com.groupdocs.parser.data/highlightitem).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | позиция | int | Позиция в тексте документа. |
|
|  | текст | java.lang.String | Текст выделения. |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


Получает позицию в тексте документа.


**Returns:**
int - Ноль-основанный индекс начальной позиции выделения.

### getText() {#getText--}
```
public String getText()
```


Получает текст выделения.


**Returns:**
java.lang.String - Строковое значение, представляющее текст выделения.


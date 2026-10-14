---
title: "SearchResult"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет результат поиска в функции поиска."
type: docs
weight: 27
url: /ru/java/com.groupdocs.parser.data/searchresult/
---
**Inheritance:**
java.lang.Object
```
public class SearchResult
```

Представляет результат поиска в функции поиска.

Экземпляр класса SearchResult используется в качестве возвращаемого значения метода [Parser.search(String)](../../com.groupdocs.parser/parser#search-String-).
и методы [Parser.search(String, com.groupdocs.parser.options.SearchOptions)](../../com.groupdocs.parser/parser#search-String--com.groupdocs.parser.options.SearchOptions-). См. примеры использования там.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)](#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-) | Инициализирует новый экземпляр класса [SearchResult](../../com.groupdocs.parser.data/searchresult). |
|
|  | [SearchResult(int position, String text, Integer pageIndex)](#SearchResult-int-java.lang.String-java.lang.Integer-) | Инициализирует новый экземпляр класса [SearchResult](../../com.groupdocs.parser.data/searchresult). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getPosition()](#getPosition--) | Получает позицию в тексте документа. |
|
|  | [getText()](#getText--) | Возвращает текст. |
|
|  | [getPageIndex()](#getPageIndex--) | Получает индекс страницы, на которой найден текст. |
|
|  | [getLeftHighlightItem()](#getLeftHighlightItem--) | Получает левое выделение. |
|
|  | [getRightHighlightItem()](#getRightHighlightItem--) | Получает правое выделение. |
|
### SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem) {#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-}
```
public SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)
```


Инициализирует новый экземпляр класса [SearchResult](../../com.groupdocs.parser.data/searchresult).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | позиция | int | Позиция в тексте документа. |
|
|  | текст | java.lang.String | Найденный текст. |
|
|  | pageIndex | java.lang.Integer | Индекс страницы, на которой найден текст. |
|
|  | leftHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | Левое выделение. |
|
|  | rightHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | Правое выделение. |
|

### SearchResult(int position, String text, Integer pageIndex) {#SearchResult-int-java.lang.String-java.lang.Integer-}
```
public SearchResult(int position, String text, Integer pageIndex)
```


Инициализирует новый экземпляр класса [SearchResult](../../com.groupdocs.parser.data/searchresult).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | позиция | int | Позиция в тексте документа. |
|
|  | текст | java.lang.String | Найденный текст. |
|
|  | pageIndex | java.lang.Integer | Индекс страницы, на которой найден текст. |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


Получает позицию в тексте документа.


**Returns:**
int - Ноль-основанный индекс начальной позиции результата поиска.

### getText() {#getText--}
```
public String getText()
```


Возвращает текст.


**Returns:**
java.lang.String - Строковое значение, представляющее найденный текст.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Получает индекс страницы, на которой найден текст.


**Returns:**
java.lang.Integer - Ноль-основанный индекс страницы, на которой найден текст; null, если поиск выполняется по всему тексту документа.

### getLeftHighlightItem() {#getLeftHighlightItem--}
```
public HighlightItem getLeftHighlightItem()
```


Получает левое выделение.


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

### getRightHighlightItem() {#getRightHighlightItem--}
```
public HighlightItem getRightHighlightItem()
```


Получает правое выделение.


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.


---
title: "OcrEventHandler"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет обработчик для событий OCR."
type: docs
weight: 26
url: /ru/java/com.groupdocs.parser.options/ocreventhandler/
---
**Inheritance:**
java.lang.Object
```
public class OcrEventHandler
```

Предоставляет обработчик для событий OCR.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [OcrEventHandler()](#OcrEventHandler--) | Инициализирует новый экземпляр класса [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getWarnings()](#getWarnings--) | Получает список сообщений предупреждений. |
|
|  | [hasWarnings()](#hasWarnings--) | Получает значение, указывающее, не пустой ли список предупреждений. |
|
|  | [getWarnings(int pageIndex)](#getWarnings-int-) | Возвращает список предупреждающих сообщений для страницы с индексом pageIndex. |
|
|  | [onWarnings(int pageIndex, Iterable<String> warnings)](#onWarnings-int-java.lang.Iterable-java.lang.String--) | Устанавливает предупреждающие сообщения для страницы. |
|
### OcrEventHandler() {#OcrEventHandler--}
```
public OcrEventHandler()
```


Инициализирует новый экземпляр класса [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


### getWarnings() {#getWarnings--}
```
public List<String> getWarnings()
```


Получает список сообщений предупреждений.


**Returns:**
java.util.List<java.lang.String> - Список предупреждающих сообщений для всех страниц.

### hasWarnings() {#hasWarnings--}
```
public boolean hasWarnings()
```


Получает значение, указывающее, не пустой ли список предупреждений.


**Returns:**
boolean -  true  если список предупреждений не пуст; иначе,  false .

### getWarnings(int pageIndex) {#getWarnings-int-}
```
public List<String> getWarnings(int pageIndex)
```


Возвращает список предупреждающих сообщений для страницы с индексом pageIndex.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pageIndex | int | Индекс страницы, начинающийся с нуля. |
|

**Returns:**
java.util.List<java.lang.String> - Список предупреждающих сообщений для страницы; пустой список, если нет предупреждающих сообщений для страницы.

### onWarnings(int pageIndex, Iterable<String> warnings) {#onWarnings-int-java.lang.Iterable-java.lang.String--}
```
public void onWarnings(int pageIndex, Iterable<String> warnings)
```


Устанавливает предупреждающие сообщения для страницы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pageIndex | int | Индекс страницы, начинающийся с нуля. |
|
|  | warnings | java.lang.Iterable<java.lang.String> | Список предупреждающих сообщений для страницы. |
|


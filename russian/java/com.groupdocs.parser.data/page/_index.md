---
title: "Page"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет информацию о странице документа, такую как индекс страницы и размер страницы."
type: docs
weight: 16
url: /ru/java/com.groupdocs.parser.data/page/
---
**Inheritance:**
java.lang.Object
```
public class Page
```

Представляет информацию о странице документа, такую как индекс страницы и размер страницы. Используется для представления страницы, содержащей наследников класса [PageArea](../../com.groupdocs.parser.data/pagearea) в функциональности парсинга по шаблону.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [Page(int index, Size size)](#Page-int-com.groupdocs.parser.data.Size-) | Создаёт новый экземпляр класса [Page](../../com.groupdocs.parser.data/page). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getIndex()](#getIndex--) | Возвращает индекс страницы. |
|
|  | [getSize()](#getSize--) | Возвращает размер страницы. |
|
### Page(int index, Size size) {#Page-int-com.groupdocs.parser.data.Size-}
```
public Page(int index, Size size)
```


Создаёт новый экземпляр класса [Page](../../com.groupdocs.parser.data/page).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | индекс | int | Индекс страницы. |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | Размер страницы. |
|

### getIndex() {#getIndex--}
```
public int getIndex()
```


Возвращает индекс страницы.


**Returns:**
int - Индекс страницы, начинающийся с нуля.

### getSize() {#getSize--}
```
public Size getSize()
```


Возвращает размер страницы.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the page.


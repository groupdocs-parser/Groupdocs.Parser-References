---
title: "DocumentPageData"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет данные страницы документа."
type: docs
weight: 12
url: /ru/java/com.groupdocs.parser.data/documentpagedata/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.DocumentData](../../com.groupdocs.parser.data/documentdata)
```
public class DocumentPageData extends DocumentData
```

Представляет данные страницы документа. Состоит из объектов [FieldData](../../com.groupdocs.parser.data/fielddata), которые содержат данные полей со страницы документа.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [DocumentPageData(Iterable<FieldData> fields, int pageIndex)](#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-) | Инициализирует новый экземпляр класса [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getPageIndex()](#getPageIndex--) | Возвращает индекс страницы. |
|
### DocumentPageData(Iterable<FieldData> fields, int pageIndex) {#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-}
```
public DocumentPageData(Iterable<FieldData> fields, int pageIndex)
```


Инициализирует новый экземпляр класса [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | поля | java.lang.Iterable<com.groupdocs.parser.data.FieldData> | Коллекция данных полей. |
|
|  | pageIndex | int | Индекс страницы, начинающийся с нуля. |
|

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Возвращает индекс страницы.


**Returns:**
int - Индекс страницы, начинающийся с нуля.


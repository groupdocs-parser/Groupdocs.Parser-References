---
title: "DocumentInfo"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет информацию о документе."
type: docs
weight: 11
url: /ru/java/com.groupdocs.parser.options/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.parser.options.IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo)
```
public abstract class DocumentInfo implements IDocumentInfo
```

Представляет информацию о документе.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getFileType()](#getFileType--) | Получает тип документа. |
|
|  | [getPageCount()](#getPageCount--) | Возвращает общее количество страниц документа. |
|
|  | [getRawPageCount()](#getRawPageCount--) | Возвращает общее количество необработанных страниц документа. |
|
|  | [getSize()](#getSize--) | Получает размер документа в байтах. |
|
|  | [getPages()](#getPages--) | Возвращает информацию о страницах, такую как индекс и размер страницы. |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


Получает тип документа.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getPageCount() {#getPageCount--}
```
public abstract int getPageCount()
```


Возвращает общее количество страниц документа.


**Returns:**
int — целочисленное значение, представляющее общее количество страниц.

### getRawPageCount() {#getRawPageCount--}
```
public abstract int getRawPageCount()
```


Возвращает общее количество необработанных страниц документа.

Используйте свойство [getRawPageCount()](../../com.groupdocs.parser.options/documentinfo#getRawPageCount--) вместо свойства [getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) для извлечения необработанного текста.
В некоторых документах номера страниц различаются в режимах точного и необработанного извлечения текста.
[getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) property may perform extra calculations which impacts on text extraction speed in raw mode.


**Returns:**
int — целочисленное значение, представляющее общее количество необработанных страниц.

### getSize() {#getSize--}
```
public abstract long getSize()
```


Получает размер документа в байтах.


**Returns:**
long - Целочисленное значение, представляющее размер документа в байтах.

### getPages() {#getPages--}
```
public abstract List<PageInfo> getPages()
```


Возвращает информацию о страницах, такую как индекс и размер страницы.


**Returns:**
java.util.List<com.groupdocs.parser.options.PageInfo> — коллекция экземпляров классов [PageInfo](../../com.groupdocs.parser.options/pageinfo).


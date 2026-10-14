---
title: "MetadataItem"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет элемент метаданных, который используется в элементах контейнера и функции извлечения метаданных."
type: docs
weight: 15
url: /ru/java/com.groupdocs.parser.data/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

Представляет элемент метаданных, который используется в элементах контейнера и функции извлечения метаданных.

Экземпляр класса [MetadataItem](../../com.groupdocs.parser.data/metadataitem) используется в качестве возвращаемого значения метода [Parser.getMetadata()](../../com.groupdocs.parser/parser#getMetadata--).
и как элемент в коллекции [ContainerItem.getMetadata()](../../com.groupdocs.parser.data/containeritem#getMetadata--). См. примеры использования там.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [MetadataItem(String name, String value)](#MetadataItem-java.lang.String-java.lang.String-) | Инициализирует новый экземпляр класса [MetadataItem](../../com.groupdocs.parser.data/metadataitem). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getName()](#getName--) | Возвращает имя элемента метаданных. |
|
|  | [getValue()](#getValue--) | Возвращает значение элемента метаданных. |
|
### MetadataItem(String name, String value) {#MetadataItem-java.lang.String-java.lang.String-}
```
public MetadataItem(String name, String value)
```


Инициализирует новый экземпляр класса [MetadataItem](../../com.groupdocs.parser.data/metadataitem).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | имя | java.lang.String | Имя элемента метаданных. |
|
|  | значение | java.lang.String | Значение элемента метаданных. |
|

### getName() {#getName--}
```
public String getName()
```


Возвращает имя элемента метаданных.


**Returns:**
java.lang.String — строковое значение, представляющее имя элемента метаданных.

### getValue() {#getValue--}
```
public String getValue()
```


Возвращает значение элемента метаданных.


**Returns:**
java.lang.String — строковое значение, представляющее значение элемента метаданных.


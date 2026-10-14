---
title: "PageTableAreaCell"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет ячейку таблицы, используемую в классе."
type: docs
weight: 23
url: /ru/java/com.groupdocs.parser.data/pagetableareacell/
---
**Inheritance:**
java.lang.Object
```
public class PageTableAreaCell
```

Представляет ячейку таблицы, используемую в классе [PageTableArea](../../com.groupdocs.parser.data/pagetablearea).

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-) | Инициализирует новый экземпляр класса [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell). |
|
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-) | Инициализирует новый экземпляр класса [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getRowIndex()](#getRowIndex--) | Получает индекс строки. |
|
|  | [getColumnIndex()](#getColumnIndex--) | Получает индекс столбца. |
|
|  | [getRowSpan()](#getRowSpan--) | Получает общее количество строк, содержащих ячейку таблицы. |
|
|  | [getColumnSpan()](#getColumnSpan--) | Получает общее количество столбцов, содержащих ячейку таблицы. |
|
|  | [getPageArea()](#getPageArea--) | Получает значение ячейки таблицы. |
|
|  | [getText()](#getText--) | Получает текстовое значение ячейки таблицы. |
|
### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)
```


Инициализирует новый экземпляр класса [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rowIndex | int | Индекс строки, начинающийся с нуля. |
|
|  | columnIndex | int | Индекс столбца, начинающийся с нуля. |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | Значение ячейки таблицы. |
|

### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)
```


Инициализирует новый экземпляр класса [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rowIndex | int | Индекс строки, начинающийся с нуля. |
|
|  | columnIndex | int | Индекс столбца, начинающийся с нуля. |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | Значение ячейки таблицы. |
|
|  | rowSpan | int | Общее количество строк, содержащих ячейку таблицы. |
|
|  | columnSpan | int | Общее количество столбцов, содержащих ячейку таблицы. |
|

### getRowIndex() {#getRowIndex--}
```
public int getRowIndex()
```


Получает индекс строки.


**Returns:**
int — нулевой индекс первой строки, содержащей ячейку таблицы.

### getColumnIndex() {#getColumnIndex--}
```
public int getColumnIndex()
```


Получает индекс столбца.


**Returns:**
int — нулевой индекс первого столбца, содержащего ячейку таблицы.

### getRowSpan() {#getRowSpan--}
```
public int getRowSpan()
```


Получает общее количество строк, содержащих ячейку таблицы.


**Returns:**
int — положительное целое значение, представляющее общее количество строк, содержащих ячейку таблицы.

### getColumnSpan() {#getColumnSpan--}
```
public int getColumnSpan()
```


Получает общее количество столбцов, содержащих ячейку таблицы.


**Returns:**
int — положительное целое значение, представляющее общее количество столбцов, содержащих ячейку таблицы.

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


Получает значение ячейки таблицы.


**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - Depending on cell [PageArea](../../com.groupdocs.parser.data/pagearea) property can contain any of the inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class.

### getText() {#getText--}
```
public String getText()
```


Получает текстовое значение ячейки таблицы.


**Returns:**
java.lang.String - Строка, представляющая текстовое значение ячейки;  null  если ячейка не содержит текстового значения.


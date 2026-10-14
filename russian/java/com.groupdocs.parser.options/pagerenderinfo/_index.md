---
title: "PageRenderInfo"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет информацию о том, как отображается страница."
type: docs
weight: 30
url: /ru/java/com.groupdocs.parser.options/pagerenderinfo/
---
**Inheritance:**
java.lang.Object
```
public class PageRenderInfo
```

Представляет информацию о том, как отображается страница.

Некоторые документы (например, электронные таблицы) невозможно отобразить страницу
в виде единого изображения. Для таких документов страница отображается как набор плиток.
Эти плитки размещаются в прямоугольной таблице.


RowCount
и
ColumnCount
представляют общее количество строк и столбцов
этой таблицы. Если страница документа отрисовывается в виде единого изображения, эти свойства равны 1.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [PageRenderInfo(int pageNumber, int rowCount, int columnCount)](#PageRenderInfo-int-int-int-) | Инициализирует новый экземпляр класса [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | Получает номер страницы. |
|
|  | [getRowCount()](#getRowCount--) | Получить общее количество строк плиток. |
|
|  | [getColumnCount()](#getColumnCount--) | Получить общее количество столбцов плиток. |
|
|  | [getColumn(int tileIndex)](#getColumn-int-) | Возвращает индекс столбца, где размещена плитка с  tileIndex . |
|
|  | [getRow(int tileIndex)](#getRow-int-) | Возвращает индекс строки, где размещена плитка с  tileIndex . |
|
### PageRenderInfo(int pageNumber, int rowCount, int columnCount) {#PageRenderInfo-int-int-int-}
```
public PageRenderInfo(int pageNumber, int rowCount, int columnCount)
```


Инициализирует новый экземпляр класса [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pageNumber | int | Номер страницы (начинается с 1). |
|
|  | rowCount | int | Общее количество строк плиток. |
|
|  | columnCount | int | Общее количество столбцов плиток. |
|

### getPageNumber() {#getPageNumber--}
```
public int getPageNumber()
```


Получает номер страницы.


**Returns:**
int - Целочисленное значение, представляющее номер страницы (начинается с 1).

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Получить общее количество строк плиток.


**Returns:**
int - Целочисленное значение, представляющее общее количество строк плиток.

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Получить общее количество столбцов плиток.


**Returns:**
int - Целочисленное значение, представляющее общее количество столбцов плиток.

### getColumn(int tileIndex) {#getColumn-int-}
```
public int getColumn(int tileIndex)
```


Возвращает индекс столбца, где размещена плитка с  tileIndex .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | tileIndex | int | Индекс плитки, начинающийся с нуля. |
|

**Returns:**
int - Целочисленное значение, начинающееся с нуля, представляющее индекс столбца.

### getRow(int tileIndex) {#getRow-int-}
```
public int getRow(int tileIndex)
```


Возвращает индекс строки, где размещена плитка с  tileIndex .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | tileIndex | int | Индекс плитки, начинающийся с нуля. |
|

**Returns:**
int - Целочисленное значение, начинающееся с нуля, представляющее индекс строки.


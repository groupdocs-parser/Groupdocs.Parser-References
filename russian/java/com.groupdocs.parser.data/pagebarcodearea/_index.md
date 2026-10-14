---
title: "PageBarcodeArea"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет область штрих‑кода на странице, которая используется для представления значения штрих‑кода в функции разбора по шаблону."
type: docs
weight: 18
url: /ru/java/com.groupdocs.parser.data/pagebarcodearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageBarcodeArea extends PageArea
```

Представляет область штрих‑кода на странице, которая используется для представления значения штрих‑кода в функции разбора по шаблону.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)](#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Инициализирует новый экземпляр класса [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getValue()](#getValue--) | Получает значение штрихкода. |
|
|  | [getCodeTypeName()](#getCodeTypeName--) | Получает имя типа штрихкода. |
|
|  | [getConfidence()](#getConfidence--) | Получает уровень уверенности распознанного штрихкода. |
|
|  | [getAngle()](#getAngle--) | Получает угол штрихкода. |
|
### PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle) {#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)
```


Инициализирует новый экземпляр класса [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | java.lang.String | Значение штрихкода. |
|
|  | codeTypeName | java.lang.String | Имя типа штрихкода. |
|
|  | confidence | int | Уровень уверенности распознанного штрихкода. |
|
|  | angle | double | Угол штрихкода. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Страница, содержащая область штрихкода. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область, содержащая область штрихкода. |
|

### getValue() {#getValue--}
```
public String getValue()
```


Получает значение штрихкода.


**Returns:**
java.lang.String - Строковое значение, представляющее значение области штрихкода на странице.

### getCodeTypeName() {#getCodeTypeName--}
```
public String getCodeTypeName()
```


Получает имя типа штрихкода.


**Returns:**
java.lang.String - Строковое значение, представляющее имя типа штрихкода.

### getConfidence() {#getConfidence--}
```
public int getConfidence()
```


Получает уровень уверенности распознанного штрихкода.


**Returns:**
int - Целочисленное значение, представляющее уверенность распознанного штрихкода (0-100).

### getAngle() {#getAngle--}
```
public double getAngle()
```


Получает угол штрихкода.


**Returns:**
double - Дробное значение, представляющее угол штрихкода (0-360).


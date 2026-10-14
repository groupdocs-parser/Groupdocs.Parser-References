---
title: "TemplateOptions"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет параметры, используемые для парсинга с помощью функциональности шаблонов."
type: docs
weight: 17
url: /ru/java/com.groupdocs.parser.templates/templateoptions/
---
**Inheritance:**
java.lang.Object
```
public class TemplateOptions
```

Предоставляет параметры, используемые для парсинга с помощью функциональности шаблонов.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [TemplateOptions(double rectangleTolerance)](#TemplateOptions-double-) | Инициализирует новый экземпляр класса [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getRectangleTolerance()](#getRectangleTolerance--) | Получает размер границы, игнорируемой при захвате прямоугольной областью. |
|
### TemplateOptions(double rectangleTolerance) {#TemplateOptions-double-}
```
public TemplateOptions(double rectangleTolerance)
```


Инициализирует новый экземпляр класса [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rectangleTolerance | double | Размер границы, игнорируемой при захвате прямоугольной областью. Он измеряется как доля высоты текстового элемента. |
|

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


Получает размер границы, игнорируемой при захвате прямоугольной областью. Он измеряется как доля высоты текстового элемента.


**Returns:**
double - Значение типа double от 0 (без границы) до 1 (игнорировать весь элемент).


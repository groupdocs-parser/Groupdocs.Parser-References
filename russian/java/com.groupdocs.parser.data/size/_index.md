---
title: "Size"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет размер."
type: docs
weight: 28
url: /ru/java/com.groupdocs.parser.data/size/
---
**Inheritance:**
java.lang.Object
```
public class Size
```

Представляет размер.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [Size(double width, double height)](#Size-double-double-) | Инициализирует новый экземпляр класса [Size](../../com.groupdocs.parser.data/size). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getWidth()](#getWidth--) | Возвращает ширину. |
|
|  | [getHeight()](#getHeight--) | Возвращает высоту. |
|
|  | [isEmpty()](#isEmpty--) | Возвращает значение, указывающее, пустой ли размер. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Преобразует строковое представление размера в его эквивалент класса. |
|
| [toString()](#toString--) |  |
### Size(double width, double height) {#Size-double-double-}
```
public Size(double width, double height)
```


Инициализирует новый экземпляр класса [Size](../../com.groupdocs.parser.data/size).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | width | double | Ширина в пикселях. |
|
|  | height | double | Высота в пикселях. |
|

### getWidth() {#getWidth--}
```
public double getWidth()
```


Возвращает ширину.


**Returns:**
double — значение двойной точности, представляющее ширину в пикселях.

### getHeight() {#getHeight--}
```
public double getHeight()
```


Возвращает высоту.


**Returns:**
double — значение двойной точности, представляющее высоту в пикселях.

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Возвращает значение, указывающее, пустой ли размер.


**Returns:**
boolean -  true  если  ширина  и  высота  равны нулю; иначе,  false .

### parse(String s) {#parse-java.lang.String-}
```
public static Size parse(String s)
```


Преобразует строковое представление размера в его эквивалент класса. Возвращаемое значение указывает, удалось ли преобразование или нет.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | s | java.lang.String | Строка, содержащая размер для преобразования. |
|

**Returns:**
[Size](../../com.groupdocs.parser.data/size) - The instance of [Size](../../com.groupdocs.parser.data/size) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String

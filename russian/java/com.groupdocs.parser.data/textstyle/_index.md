---
title: "TextStyle"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет стиль текста, такой как название шрифта, размер шрифта и т.д."
type: docs
weight: 30
url: /ru/java/com.groupdocs.parser.data/textstyle/
---
**Inheritance:**
java.lang.Object
```
public final class TextStyle
```

Представляет стиль текста, такой как название шрифта, размер шрифта и т.д.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)](#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-) | Инициализирует новый экземпляр класса [TextStyle](../../com.groupdocs.parser.data/textstyle). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getName()](#getName--) | Возвращает название стиля. |
|
|  | [getFontName()](#getFontName--) | Возвращает название шрифта. |
|
|  | [getFontSize()](#getFontSize--) | Получает размер шрифта. |
|
|  | [isBold()](#isBold--) | Получает значение, указывающее, является ли шрифт полужирным. |
|
|  | [isItalic()](#isItalic--) | Получает значение, указывающее, является ли шрифт курсивным. |
|
| [equals(Object o)](#equals-java.lang.Object-) |  |
| [hashCode()](#hashCode--) |  |
### TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic) {#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-}
```
public TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)
```


Инициализирует новый экземпляр класса [TextStyle](../../com.groupdocs.parser.data/textstyle).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | имя | java.lang.String | Имя стиля. |
|
|  | fontName | java.lang.String | Имя шрифта. |
|
|  | fontSize | double | Размер шрифта. |
|
|  | bold | boolean | Значение, указывающее, является ли шрифт полужирным. |
|
|  | italic | boolean | Значение, указывающее, является ли шрифт курсивным. |
|

### getName() {#getName--}
```
public String getName()
```


Возвращает название стиля.


**Returns:**
java.lang.String - Строковое значение, представляющее имя стиля.

### getFontName() {#getFontName--}
```
public String getFontName()
```


Возвращает название шрифта.


**Returns:**
java.lang.String - Строковое значение, представляющее имя шрифта.

### getFontSize() {#getFontSize--}
```
public double getFontSize()
```


Получает размер шрифта.


**Returns:**
double - Значение типа double, представляющее размер шрифта.

### isBold() {#isBold--}
```
public boolean isBold()
```


Получает значение, указывающее, является ли шрифт полужирным.


**Returns:**
boolean -  true  если шрифт полужирный; иначе,  false .

### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Получает значение, указывающее, является ли шрифт курсивным.


**Returns:**
boolean -  true  если шрифт курсивный; иначе,  false .

### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object |  |

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int

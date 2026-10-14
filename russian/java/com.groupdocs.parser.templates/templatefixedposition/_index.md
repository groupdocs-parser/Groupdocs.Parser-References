---
title: "TemplateFixedPosition"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет позицию поля шаблона, определяемую прямоугольной областью."
type: docs
weight: 13
url: /ru/java/com.groupdocs.parser.templates/templatefixedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateFixedPosition extends TemplatePosition
```

Предоставляет позицию поля шаблона, определяемую прямоугольной областью.

Это самый простой способ определить позицию поля. Требуется задать прямоугольную область на странице, которая ограничивает
значение поля. Весь текст, содержащийся (даже частично) в прямоугольной области, будет извлечён как значение:

````
// Create a fixed template field with "Address" name which is bounded by a rectangle at the position (35, 160) and with the size (110, 20)
 TemplateField templateField = new TemplateField(
     new TemplateFixedPosition(new Rectangle(new Point(35, 160), new Size(110, 20))),
     "Address");
 
````


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [TemplateFixedPosition(Rectangle rectangle)](#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-) | Инициализирует новый экземпляр класса [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Получает прямоугольную область, содержащую шаблонное поле. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateFixedPosition(Rectangle rectangle) {#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-}
```
public TemplateFixedPosition(Rectangle rectangle)
```


Инициализирует новый экземпляр класса [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область, содержащая шаблонное поле. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Получает прямоугольную область, содержащую шаблонное поле.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template field.

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


Создаёт копию текущей позиции со всеми координатами, масштабированными на заданный коэффициент.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| коэффициент | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)

---
title: "TemplateRegexPosition"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет позицию поля шаблона, использующую регулярное выражение."
type: docs
weight: 19
url: /ru/java/com.groupdocs.parser.templates/templateregexposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateRegexPosition extends TemplatePosition
```

Предоставляет позицию поля шаблона, использующую регулярное выражение.

Следующий пример показывает ситуацию, если документ содержит \"Invoice Number INV-12345\"
тогда поле шаблона можно определить следующим образом:

````
// Create a regex template field with "InvoiceNumber" name
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+[A-Z0-9\\-]+"),
     "InvoiceNumber");
 
````

В этом случае в качестве значения извлекается вся строка. Чтобы извлечь только часть строки
используется группа регулярного выражения \"value\":

````
// Create a regex template field with "InvoiceNumber" name with "value" group
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+(?[A-Z0-9\\-]+)"),
     "InvoiceNumber");
````

В этом случае в качестве значения извлекается строка \"INV-3337\".

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [TemplateRegexPosition(String expression)](#TemplateRegexPosition-java.lang.String-) | Инициализирует новый экземпляр класса [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition). |
|
|  | [TemplateRegexPosition(String expression, boolean matchCase)](#TemplateRegexPosition-java.lang.String-boolean-) | Инициализирует новый экземпляр класса [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getExpression()](#getExpression--) | Возвращает регулярное выражение. |
|
|  | [isMatchCase()](#isMatchCase--) | Возвращает значение, что регистр текста не игнорируется. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateRegexPosition(String expression) {#TemplateRegexPosition-java.lang.String-}
```
public TemplateRegexPosition(String expression)
```


Инициализирует новый экземпляр класса [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | expression | java.lang.String | Регулярное выражение. |
|

### TemplateRegexPosition(String expression, boolean matchCase) {#TemplateRegexPosition-java.lang.String-boolean-}
```
public TemplateRegexPosition(String expression, boolean matchCase)
```


Инициализирует новый экземпляр класса [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | expression | java.lang.String | Регулярное выражение. |
|
|  | matchCase | boolean | Значение, указывающее, не игнорируется ли регистр текста. |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


Возвращает регулярное выражение.


**Returns:**
java.lang.String — строка, представляющая регулярное выражение.

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Возвращает значение, что регистр текста не игнорируется.


**Returns:**
boolean — true, если регистр текста не игнорируется; иначе false.

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

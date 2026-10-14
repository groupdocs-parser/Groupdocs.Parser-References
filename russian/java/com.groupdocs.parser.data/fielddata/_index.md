---
title: "FieldData"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет данные поля, такие как имя, индекс страницы, значение поля и т.д."
type: docs
weight: 13
url: /ru/java/com.groupdocs.parser.data/fielddata/
---
**Inheritance:**
java.lang.Object
```
public class FieldData
```

Представляет данные поля, такие как имя, индекс страницы, значение поля и т.д. В зависимости от поля значение может быть текстом, изображением, таблицей и т.п.

Экземпляры класса [FieldData](../../com.groupdocs.parser.data/fielddata) используются в коллекции [DocumentData](../../com.groupdocs.parser.data/documentdata).

## Методы

| Метод | Описание |
| --- | --- |
|  | [getName()](#getName--) | Возвращает имя поля. |
|
|  | [getPageIndex()](#getPageIndex--) | Возвращает индекс страницы. |
|
|  | [getPageArea()](#getPageArea--) | Возвращает значение поля. |
|
|  | [getLinkedField()](#getLinkedField--) | Возвращает связанное поле. |
|
|  | [getText()](#getText--) | Возвращает текст. |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | Получает значение, указывающее, было ли  Name  преобразовано в ВЕРХНИЙ РЕГИСТР. |
|
### getName() {#getName--}
```
public String getName()
```


Возвращает имя поля.


**Returns:**
java.lang.String — строковое значение в верхнем регистре, представляющее имя поля.

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Возвращает индекс страницы.


**Returns:**
int — нулевой индекс страницы, содержащей поле.

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


Возвращает значение поля.

В зависимости от поля свойство PageArea может содержать любой из наследников класса [PageArea](../../com.groupdocs.parser.data/pagearea).
Например, метод [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) извлекает только текстовые поля.

````
PageTextArea area = field.getPageArea() instanceof PageTextArea
         ? (PageTextArea) field.getPageArea()
         : null;
 System.out.println(area == null ? "Not a template field" : area.getText());
 
````



**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - An instance of [PageArea](../../com.groupdocs.parser.data/pagearea) class that represents the value of the field.

### getLinkedField() {#getLinkedField--}
```
public FieldData getLinkedField()
```


Возвращает связанное поле.


**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class that represents the field which is linked to the field;  null  if it isn't set.

### getText() {#getText--}
```
public String getText()
```


Возвращает текст.


**Returns:**
java.lang.String — строковое значение, представляющее текстовое значение поля; null, если свойство [PageArea](../../com.groupdocs.parser.data/pagearea) не является [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


Получает значение, указывающее, было ли  Name  преобразовано в ВЕРХНИЙ РЕГИСТР.


**Returns:**
boolean - Булево значение, указывающее, было ли  Name  преобразовано в ВЕРХНИЙ РЕГИСТР.


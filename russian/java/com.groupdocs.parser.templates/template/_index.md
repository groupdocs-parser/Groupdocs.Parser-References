---
title: "Template"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет шаблон страницы документа."
type: docs
weight: 10
url: /ru/java/com.groupdocs.parser.templates/template/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Template implements Iterable<TemplateItem>
```

Предоставляет шаблон страницы документа. Он состоит из объектов [TemplateItem](../../com.groupdocs.parser/templates/templateitem), представляющих элементы шаблона, такие как текстовое поле и определения таблиц.

**Learn more:**

* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [Template(Iterable<? extends TemplateItem> items)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--) | Инициализирует новый экземпляр класса [Template](../../com.groupdocs.parser.templates/template). |
|
|  | [Template(Iterable<? extends TemplateItem> items, TemplateOptions options)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-) | Инициализирует новый экземпляр класса [Template](../../com.groupdocs.parser.templates/template). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getCount()](#getCount--) | Получает общее количество элементов шаблона. |
|
|  | [get(int index)](#get-int-) | Получает элемент шаблона по индексу. |
|
|  | [getOptions()](#getOptions--) | Получает параметры шаблона. |
|
| [iterator()](#iterator--) |  |
|  | [load(String filePath)](#load-java.lang.String-) | Загружает шаблон из файла. |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | Загружает шаблон из потока. |
|
|  | [save(String filePath)](#save-java.lang.String-) | Сохраняет шаблон в файл. |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | Сохраняет шаблон в поток. |
|
### Template(Iterable<? extends TemplateItem> items) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--}
```
public Template(Iterable<? extends TemplateItem> items)
```


Инициализирует новый экземпляр класса [Template](../../com.groupdocs.parser.templates/template).

Использование:

````
// Create an array of template fields
 TemplateItem[] fields = new TemplateItem[]
 {
     new TemplateField(new TemplateRegexPosition("From"), "From", 0),
     new TemplateField(
         new TemplateLinkedPosition("From", new Size(100, 10), new TemplateLinkedPositionEdges(false, false, false, true)),
         "FromCompany",
         0),
     new TemplateField(
         new TemplateLinkedPosition("FromCompany", new Size(100, 30), new TemplateLinkedPositionEdges(false, false, false, true)),
         "FromAddress",
         0)
 };
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(fields));
 
````



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | Коллекция объектов [TemplateItem](../../com.groupdocs.parser.templates/templateitem). |
|

### Template(Iterable<? extends TemplateItem> items, TemplateOptions options) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-}
```
public Template(Iterable<? extends TemplateItem> items, TemplateOptions options)
```


Инициализирует новый экземпляр класса [Template](../../com.groupdocs.parser.templates/template).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | Коллекция объектов [TemplateItem](../../com.groupdocs.parser.templates/templateitem). |
|
|  | options | [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) | Параметры шаблона. |
|

### getCount() {#getCount--}
```
public int getCount()
```


Получает общее количество элементов шаблона.


**Returns:**
int — целое число, представляющее общее количество элементов шаблона.

### get(int index) {#get-int-}
```
public TemplateItem get(int index)
```


Получает элемент шаблона по индексу.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | индекс | int | Индекс элемента шаблона, начинающийся с нуля. |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - An instance of [TemplateItem](../../com.groupdocs.parser.templates/templateitem) class.

### getOptions() {#getOptions--}
```
public TemplateOptions getOptions()
```


Получает параметры шаблона.


**Returns:**
[TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) - An instance of [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) class.

### iterator() {#iterator--}
```
public Iterator<TemplateItem> iterator()
```




**Returns:**
java.util.Iterator<com.groupdocs.parser.templates.TemplateItem>
### load(String filePath) {#load-java.lang.String-}
```
public static Template load(String filePath)
```


Загружает шаблон из файла.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Путь к файлу. |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Template load(InputStream stream)
```


Загружает шаблон из потока.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | stream | java.io.InputStream | Входной поток. |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


Сохраняет шаблон в файл.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Путь к файлу. |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Сохраняет шаблон в поток.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | stream | java.io.OutputStream | Поток вывода. |
|


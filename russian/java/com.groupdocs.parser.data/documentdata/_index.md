---
title: "DocumentData"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет данные документа."
type: docs
weight: 11
url: /ru/java/com.groupdocs.parser.data/documentdata/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class DocumentData implements Iterable<FieldData>
```

Представляет данные документа. Он состоит из объектов [FieldData](../../com.groupdocs.parser.data/fielddata), которые содержат данные полей из документа. Экземпляр класса [DocumentData](../../com.groupdocs.parser.data/documentdata) используется в качестве возвращаемого значения методов [Parser.parseByTemplate(Template)](../../com.groupdocs.parser/parser#parseByTemplate-Template-) и [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) . См. примеры использования там.

## Методы

| Метод | Описание |
| --- | --- |
|  | [getTemplate()](#getTemplate--) | Получает шаблон, который создал эти данные документа. |
|
|  | [getCount()](#getCount--) | Получает общее количество данных полей. |
|
|  | [get(int index)](#get-int-) | Получает данные поля по индексу. |
|
|  | [getFieldsByName(String fieldName)](#getFieldsByName-java.lang.String-) | Возвращает коллекцию данных полей, где имя равно  fieldName . |
|
|  | [iterator()](#iterator--) | Возвращает итератор по элементам этого списка в правильной последовательности. |
|
### getTemplate() {#getTemplate--}
```
public Template getTemplate()
```


Получает шаблон, который создал эти данные документа.

Когда данные были получены в результате автоматического выбора шаблона-коллекции (см
[Parser.parseByTemplate(com.groupdocs.parser.templates.TemplateCollection, com.groupdocs.parser.options.ParseByTemplateOptions)](../../com.groupdocs.parser/parser#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection--com.groupdocs.parser.options.ParseByTemplateOptions-)),
это выбранный шаблон.
null
когда данные не были получены из шаблона.


**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - The source [Template](../../com.groupdocs.parser.templates/template), or  null .

### getCount() {#getCount--}
```
public int getCount()
```


Получает общее количество данных полей.


**Returns:**
int — целочисленное значение, представляющее общее количество данных полей.

### get(int index) {#get-int-}
```
public FieldData get(int index)
```


Получает данные поля по индексу.

Итерация по всем полям:

````
// Print all extracted data
 for (int i = 0; i < data.getCount(); i++) {
     // Print field name
     System.out.print(data.get(i).getName() + ": ");
     // As we have defined only text fields in the template,
     // we cast PageArea property value to PageTextArea
     PageTextArea area = data.get(i).getPageArea() instanceof PageTextArea
             ? (PageTextArea) data.get(i).getPageArea()
             : null;
     System.out.println(area == null ? "Not a template field" : area.getText());
 }
 
````

[FieldData](../../com.groupdocs.parser.data/fielddata) class represents field data. Depending on the field PageArea property can contain any
наследников класса [PageArea](../../com.groupdocs.parser.data/pagearea). Например, метод [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) извлекает только текстовые поля:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleFormsPdf)) {
     // Extract data from PDF document
     DocumentData data = parser.parseForm();
     // Check if form extraction is supported
     if (data == null) {
         System.out.println("Form extraction isn't supported.");
         return;
     }
     // Iterate over extracted data
     for (int i = 0; i < data.getCount(); i++) {
         System.out.print(data.get(i).getName() + ": ");
         PageTextArea area = data.get(i).getPageArea() instanceof PageTextArea
                 ? (PageTextArea) data.get(i).getPageArea()
                 : null;
         System.out.println(area == null ? "Not a template field" : area.getText());
     }
 }
 
````



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | индекс | int | Нулевой индекс поля. |
|

**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class.

### getFieldsByName(String fieldName) {#getFieldsByName-java.lang.String-}
```
public List<FieldData> getFieldsByName(String fieldName)
```


Возвращает коллекцию данных полей, где имя равно  fieldName .

Найдите поля по имени поля:

````
// Print prices
 System.out.println("Prices:");
 for (FieldData field : data.getFieldsByName("Price")) {
     PageTextArea area = field.getPageArea() instanceof PageTextArea
             ? (PageTextArea) field.getPageArea()
             : null;
     System.out.println(area == null ? "Not a template field" : area.getText());
 }
 
````

[FieldData](../../com.groupdocs.parser.data/fielddata) class represents field data. Depending on the field [PageArea](../../com.groupdocs.parser.data/pagearea) property can contain
любой из наследников класса [PageArea](../../com.groupdocs.parser.data/pagearea). Например, метод [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) извлекает только текстовые поля.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | fieldName | java.lang.String | Имя поля. |
|

**Returns:**
java.util.List<com.groupdocs.parser.data.FieldData> — коллекция объектов [FieldData](../../com.groupdocs.parser.data/fielddata); пустая коллекция, если данные полей не найдены.

### iterator() {#iterator--}
```
public Iterator<FieldData> iterator()
```


Возвращает итератор по элементам этого списка в правильной последовательности.


**Returns:**
java.util.Iterator<com.groupdocs.parser.data.FieldData> — итератор по элементам этого списка в правильном порядке.


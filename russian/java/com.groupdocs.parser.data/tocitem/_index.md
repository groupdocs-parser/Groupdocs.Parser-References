---
title: "TocItem"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет элемент, который используется в функции извлечения оглавления."
type: docs
weight: 31
url: /ru/java/com.groupdocs.parser.data/tocitem/
---
**Inheritance:**
java.lang.Object
```
public class TocItem
```

Представляет элемент, который используется в функции извлечения оглавления.

Экземпляр класса [TocItem](../../com.groupdocs.parser.data/tocitem) используется в качестве возвращаемого значения метода [Parser.getToc()](../../com.groupdocs.parser/parser#getToc--). См. примеры использования там.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [TocItem(int depth, String text, Integer pageIndex)](#TocItem-int-java.lang.String-java.lang.Integer-) | Инициализирует новый экземпляр класса TocItem. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getDepth()](#getDepth--) | Возвращает уровень глубины. |
|
|  | [getText()](#getText--) | Возвращает текст. |
|
|  | [getPageIndex()](#getPageIndex--) | Возвращает индекс страницы. |
|
|  | [extractText()](#extractText--) | Извлекает текст из документа, к которому относится объект TocItem. |
|
### TocItem(int depth, String text, Integer pageIndex) {#TocItem-int-java.lang.String-java.lang.Integer-}
```
public TocItem(int depth, String text, Integer pageIndex)
```


Инициализирует новый экземпляр класса TocItem.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | depth | int | Уровень глубины элемента. |
|
|  | текст | java.lang.String | Текст элемента. |
|
|  | pageIndex | java.lang.Integer | Индекс страницы, на которую ссылается элемент |
|

### getDepth() {#getDepth--}
```
public int getDepth()
```


Возвращает уровень глубины.


**Returns:**
int — целочисленное значение, представляющее уровень глубины элемента.

### getText() {#getText--}
```
public String getText()
```


Возвращает текст.


**Returns:**
java.lang.String — строковое значение, представляющее текст элемента.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Возвращает индекс страницы.


**Returns:**
java.lang.Integer — целочисленное значение, представляющее индекс страницы, на которую ссылается элемент;  null  если оно не установлено.

### extractText() {#extractText--}
```
public TextReader extractText()
```


Извлекает текст из документа, к которому относится объект TocItem.

Следующий пример показывает, как извлечь текст с помощью элемента оглавления:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleDocxWithToc)) {
     // Get table of contents
     Iterable tocItems = parser.getToc();

     // Check if toc extraction is supported
     if (tocItems == null) {
         System.out.println("Table of contents extraction isn't supported");
     }

     // Iterate over items
     for (TocItem tocItem : tocItems) {
         // Print the text of the chapter
         try (TextReader reader = tocItem.extractText()) {
             System.out.println("----");
             System.out.println(reader.readToEnd());
         }
     }
 }
 
````



**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text.


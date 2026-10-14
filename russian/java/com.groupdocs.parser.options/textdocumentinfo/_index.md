---
title: "TextDocumentInfo"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет информацию о текстовом документе."
type: docs
weight: 36
url: /ru/java/com.groupdocs.parser.options/textdocumentinfo/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.DocumentInfo](../../com.groupdocs.parser.options/documentinfo)
```
public abstract class TextDocumentInfo extends DocumentInfo
```

Представляет информацию о текстовом документе.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [TextDocumentInfo()](#TextDocumentInfo--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getCharset()](#getCharset--) | Получает обнаруженную кодировку текстового документа. |
|
### TextDocumentInfo() {#TextDocumentInfo--}
```
public TextDocumentInfo()
```


### getCharset() {#getCharset--}
```
public abstract Charset getCharset()
```


Получает обнаруженную кодировку текстового документа.


**Returns:**
java.nio.charset.Charset - Экземпляр класса Charset.


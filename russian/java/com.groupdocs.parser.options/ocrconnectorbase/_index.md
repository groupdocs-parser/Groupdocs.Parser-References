---
title: "OcrConnectorBase"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет функциональность OCR."
type: docs
weight: 25
url: /ru/java/com.groupdocs.parser.options/ocrconnectorbase/
---
**Inheritance:**
java.lang.Object
```
public class OcrConnectorBase
```

Предоставляет функциональность OCR.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [OcrConnectorBase()](#OcrConnectorBase--) | Инициализирует новый экземпляр класса [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [isTextSupported()](#isTextSupported--) | Получает значение, указывающее, поддерживается ли извлечение текста. |
|
|  | [isTextAreasSupported()](#isTextAreasSupported--) | Получает значение, указывающее, поддерживается ли извлечение областей текста. |
|
|  | [recognizeText(InputStream imageStream, OcrOptions options)](#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-) | Распознаёт текст из  imageStream  потока. |
|
|  | [recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)](#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-) | Распознаёт области текста из  imageStream  потока. |
|
### OcrConnectorBase() {#OcrConnectorBase--}
```
public OcrConnectorBase()
```


Инициализирует новый экземпляр класса [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase).


### isTextSupported() {#isTextSupported--}
```
public boolean isTextSupported()
```


Получает значение, указывающее, поддерживается ли извлечение текста.


**Returns:**
boolean -  true  если поддерживается извлечение текста; иначе,  false .

### isTextAreasSupported() {#isTextAreasSupported--}
```
public boolean isTextAreasSupported()
```


Получает значение, указывающее, поддерживается ли извлечение областей текста.


**Returns:**
boolean -  true  если поддерживается извлечение областей текста; иначе,  false .

### recognizeText(InputStream imageStream, OcrOptions options) {#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-}
```
public String recognizeText(InputStream imageStream, OcrOptions options)
```


Распознаёт текст из  imageStream  потока.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Изображение, представляющее страницу документа. |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Параметры OCR. |
|

**Returns:**
java.lang.String - Строка, представляющая распознанный текст;  null  если распознавание текста не поддерживается.

### recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options) {#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-}
```
public Iterable<PageTextArea> recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)
```


Распознаёт области текста из  imageStream  потока.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Изображение, представляющее страницу документа. |
|
|  | pageSize | [Size](../../com.groupdocs.parser.data/size) | Размер страницы документа. |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Параметры OCR. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Коллекция объектов [PageTextArea](../../com.groupdocs.parser.data/pagetextarea);  null  если распознавание областей текста не поддерживается.


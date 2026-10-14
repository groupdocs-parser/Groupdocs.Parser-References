---
title: "Функции"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет список поддерживаемых функций."
type: docs
weight: 18
url: /ru/java/com.groupdocs.parser.options/features/
---
**Inheritance:**
java.lang.Object
```
public abstract class Features
```

Представляет список поддерживаемых функций. Позволяет получить информацию о том, какие функции поддерживаются, а какие нет, для документа.

Экземпляр этого класса используется как свойство [Parser.getFeatures()](../../com.groupdocs.parser/parser#getFeatures--). См. примеры использования там.

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Features()](#Features--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [isFeatureSupported(String featureName)](#isFeatureSupported-java.lang.String-) | Возвращает значение, указывающее, поддерживается ли функция. |
|
|  | [isText()](#isText--) | Получает значение, указывающее, поддерживается ли извлечение текста. |
|
|  | [isTextPage()](#isTextPage--) | Получает значение, указывающее, поддерживается ли извлечение страниц текста. |
|
|  | [isFormattedText()](#isFormattedText--) | Получает значение, указывающее, поддерживается ли извлечение форматированного текста. |
|
|  | [isFormattedTextPage()](#isFormattedTextPage--) | Получает значение, указывающее, поддерживается ли извлечение страниц форматированного текста. |
|
|  | [isSearch()](#isSearch--) | Получает значение, указывающее, поддерживается ли поиск текста. |
|
|  | [isHighlight()](#isHighlight--) | Получает значение, указывающее, поддерживается ли извлечение выделения. |
|
|  | [isBarcodes()](#isBarcodes--) | Получает значение, указывающее, поддерживается ли извлечение штрихкодов. |
|
|  | [isToc()](#isToc--) | Получает значение, указывающее, поддерживается ли извлечение оглавления. |
|
|  | [isMetadata()](#isMetadata--) | Получает значение, указывающее, поддерживается ли извлечение метаданных. |
|
|  | [isContainer()](#isContainer--) | Получает значение, указывающее, поддерживается ли извлечение контейнера. |
|
|  | [isTextAreas()](#isTextAreas--) | Получает значение, указывающее, поддерживается ли извлечение текстовых областей. |
|
|  | [isStructure()](#isStructure--) | Получает значение, указывающее, поддерживается ли извлечение структуры текста. |
|
|  | [isImages()](#isImages--) | Получает значение, указывающее, поддерживается ли извлечение изображений. |
|
|  | [isHyperlinks()](#isHyperlinks--) | Получает значение, указывающее, поддерживается ли извлечение гиперссылок. |
|
|  | [isTables()](#isTables--) | Получает значение, указывающее, поддерживается ли извлечение таблиц. |
|
|  | [isAnnotations()](#isAnnotations--) | Получает значение, указывающее, поддерживается ли извлечение аннотаций. |
|
|  | [isParseByTemplate()](#isParseByTemplate--) | Получает значение, указывающее, поддерживается ли разбор по шаблону. |
|
|  | [isParseForm()](#isParseForm--) | Получает значение, указывающее, поддерживается ли разбор форм. |
|
|  | [isPreview()](#isPreview--) | Получает значение, указывающее, поддерживается ли генерация предварительного просмотра. |
|
|  | [isPagePreview()](#isPagePreview--) | Получает значение, указывающее, поддерживается ли генерация предварительного просмотра страниц. |
|
|  | [isOcr()](#isOcr--) | Получает значение, указывающее, поддерживается ли функциональность OCR. |
|
|  | [isWorksheet()](#isWorksheet--) | Получает значение, указывающее, поддерживается ли извлечение листов. |
|
### Features() {#Features--}
```
public Features()
```


### isFeatureSupported(String featureName) {#isFeatureSupported-java.lang.String-}
```
public abstract boolean isFeatureSupported(String featureName)
```


Возвращает значение, указывающее, поддерживается ли функция.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | featureName | java.lang.String | Имя функции. |
|

**Returns:**
boolean -  true  если функция поддерживается; иначе,  false .

### isText() {#isText--}
```
public boolean isText()
```


Получает значение, указывающее, поддерживается ли извлечение текста.


**Returns:**
boolean -  true  если поддерживается извлечение текста; иначе,  false .

### isTextPage() {#isTextPage--}
```
public boolean isTextPage()
```


Получает значение, указывающее, поддерживается ли извлечение страниц текста.


**Returns:**
boolean -  true  если поддерживается извлечение текстовых страниц; иначе,  false .

### isFormattedText() {#isFormattedText--}
```
public boolean isFormattedText()
```


Получает значение, указывающее, поддерживается ли извлечение форматированного текста.


**Returns:**
boolean -  true  если поддерживается извлечение форматированного текста; иначе,  false .

### isFormattedTextPage() {#isFormattedTextPage--}
```
public boolean isFormattedTextPage()
```


Получает значение, указывающее, поддерживается ли извлечение страниц форматированного текста.


**Returns:**
boolean -  true  если поддерживается форматированная текстовая страница; иначе,  false .

### isSearch() {#isSearch--}
```
public boolean isSearch()
```


Получает значение, указывающее, поддерживается ли поиск текста.


**Returns:**
boolean -  true  если поддерживается поиск текста; иначе,  false .

### isHighlight() {#isHighlight--}
```
public boolean isHighlight()
```


Получает значение, указывающее, поддерживается ли извлечение выделения.


**Returns:**
boolean -  true  если поддерживается извлечение выделения; иначе,  false .

### isBarcodes() {#isBarcodes--}
```
public boolean isBarcodes()
```


Получает значение, указывающее, поддерживается ли извлечение штрихкодов.


**Returns:**
boolean -  true  если поддерживается извлечение штрихкодов; иначе,  false .

### isToc() {#isToc--}
```
public boolean isToc()
```


Получает значение, указывающее, поддерживается ли извлечение оглавления.


**Returns:**
boolean -  true  если поддерживается извлечение оглавления; иначе,  false .

### isMetadata() {#isMetadata--}
```
public boolean isMetadata()
```


Получает значение, указывающее, поддерживается ли извлечение метаданных.


**Returns:**
boolean -  true  если поддерживается извлечение метаданных; иначе,  false .

### isContainer() {#isContainer--}
```
public boolean isContainer()
```


Получает значение, указывающее, поддерживается ли извлечение контейнера.


**Returns:**
boolean -  true  если поддерживается извлечение контейнера; иначе,  false .

### isTextAreas() {#isTextAreas--}
```
public boolean isTextAreas()
```


Получает значение, указывающее, поддерживается ли извлечение текстовых областей.


**Returns:**
boolean -  true  если поддерживается извлечение текстовых областей; иначе,  false .

### isStructure() {#isStructure--}
```
public boolean isStructure()
```


Получает значение, указывающее, поддерживается ли извлечение структуры текста.


**Returns:**
boolean -  true  если поддерживается извлечение структуры текста; иначе,  false .

### isImages() {#isImages--}
```
public boolean isImages()
```


Получает значение, указывающее, поддерживается ли извлечение изображений.


**Returns:**
boolean -  true  если поддерживается извлечение изображений; иначе,  false .

### isHyperlinks() {#isHyperlinks--}
```
public boolean isHyperlinks()
```


Получает значение, указывающее, поддерживается ли извлечение гиперссылок.


**Returns:**
boolean -  true  если поддерживается извлечение гиперссылок; иначе,  false .

### isTables() {#isTables--}
```
public boolean isTables()
```


Получает значение, указывающее, поддерживается ли извлечение таблиц.


**Returns:**
boolean -  true  если поддерживается извлечение таблиц; иначе,  false .

### isAnnotations() {#isAnnotations--}
```
public boolean isAnnotations()
```


Получает значение, указывающее, поддерживается ли извлечение аннотаций.


**Returns:**
boolean -  true  если поддерживается извлечение аннотаций; иначе,  false .

### isParseByTemplate() {#isParseByTemplate--}
```
public boolean isParseByTemplate()
```


Получает значение, указывающее, поддерживается ли разбор по шаблону.


**Returns:**
boolean -  true  если поддерживается разбор по шаблону; иначе,  false .

### isParseForm() {#isParseForm--}
```
public boolean isParseForm()
```


Получает значение, указывающее, поддерживается ли разбор форм.


**Returns:**
boolean -  true  если поддерживается разбор форм; в противном случае,  false .

### isPreview() {#isPreview--}
```
public boolean isPreview()
```


Получает значение, указывающее, поддерживается ли генерация предварительного просмотра.


**Returns:**
boolean -  true  если поддерживается генерация предварительного просмотра; в противном случае,  false .

### isPagePreview() {#isPagePreview--}
```
public boolean isPagePreview()
```


Получает значение, указывающее, поддерживается ли генерация предварительного просмотра страниц.


**Returns:**
boolean -  true  если поддерживается генерация предварительного просмотра страницы; в противном случае,  false .

### isOcr() {#isOcr--}
```
public boolean isOcr()
```


Получает значение, указывающее, поддерживается ли функциональность OCR.


**Returns:**
boolean -  true  если поддерживается функция OCR; в противном случае,  false .

### isWorksheet() {#isWorksheet--}
```
public boolean isWorksheet()
```


Получает значение, указывающее, поддерживается ли извлечение листов.


**Returns:**
boolean -  true  если поддерживается извлечение листов; в противном случае,  false .


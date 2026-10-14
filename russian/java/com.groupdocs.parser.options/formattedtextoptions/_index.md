---
title: "FormattedTextOptions"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет параметры, используемые для извлечения форматированного текста."
type: docs
weight: 21
url: /ru/java/com.groupdocs.parser.options/formattedtextoptions/
---
**Inheritance:**
java.lang.Object
```
public class FormattedTextOptions
```

Предоставляет параметры, используемые для извлечения форматированного текста.

Экземпляр класса [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) используется в качестве параметра в методе [Parser.getFormattedText(FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-FormattedTextOptions-)
и методы [Parser.getFormattedText(int, FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-int--FormattedTextOptions-). См. примеры использования там.

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [FormattedTextOptions()](#FormattedTextOptions--) | Инициализирует новый экземпляр класса [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) без установленного режима. |
|
|  | [FormattedTextOptions(FormattedTextMode mode)](#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-) | Инициализирует новый экземпляр класса [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getMode()](#getMode--) | Получает режим извлечения форматированного текста. |
|
|  | [setMode(FormattedTextMode mode)](#setMode-com.groupdocs.parser.options.FormattedTextMode-) | Устанавливает режим извлечения форматированного текста. |
|
### FormattedTextOptions() {#FormattedTextOptions--}
```
public FormattedTextOptions()
```


Инициализирует новый экземпляр класса [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) без установленного режима.


### FormattedTextOptions(FormattedTextMode mode) {#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-}
```
public FormattedTextOptions(FormattedTextMode mode)
```


Инициализирует новый экземпляр класса [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | Режим извлечения форматированного текста. |
|

### getMode() {#getMode--}
```
public FormattedTextMode getMode()
```


Получает режим извлечения форматированного текста.


**Returns:**
[FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) - [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) enumeration that contains a formatted text extraction mode.

### setMode(FormattedTextMode mode) {#setMode-com.groupdocs.parser.options.FormattedTextMode-}
```
public void setMode(FormattedTextMode mode)
```


Устанавливает режим извлечения форматированного текста.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | Перечисление [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode), которое содержит режим извлечения форматированного текста. |
|


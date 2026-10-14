---
title: "TextOptions"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет параметры, используемые для извлечения текста."
type: docs
weight: 37
url: /ru/java/com.groupdocs.parser.options/textoptions/
---
**Inheritance:**
java.lang.Object
```
public class TextOptions
```

Предоставляет параметры, используемые для извлечения текста.

Экземпляр класса [TextOptions](../../com.groupdocs.parser.options/textoptions) используется в качестве параметра в методе [Parser.getText(TextOptions)](../../com.groupdocs.parser/parser#getText-TextOptions-)
и методы [Parser.getText(int, TextOptions)](../../com.groupdocs.parser/parser#getText-int--TextOptions-). См. примеры использования там.

Он используется для указания необработанного режима извлечения текста. Текст в этом режиме извлекается неточно
но быстрее, чем в стандартном режиме. Если необработанный режим не поддерживает формат документа,
то этот параметр игнорируется и используется стандартный режим.

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [TextOptions(boolean useRawModeIfPossible)](#TextOptions-boolean-) | Создаёт новый экземпляр класса [TextOptions](../../com.groupdocs.parser.options/textoptions). |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr)](#TextOptions-boolean-boolean-) | Создаёт новый экземпляр класса [TextOptions](../../com.groupdocs.parser.options/textoptions) с опцией использования OCR. |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)](#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-) | Создаёт новый экземпляр класса [TextOptions](../../com.groupdocs.parser.options/textoptions) с возможностью задавать параметры OCR. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [isUseRawModeIfPossible()](#isUseRawModeIfPossible--) | Возвращает значение, указывающее, используется ли необработанный режим. |
|
|  | [isUseOcr()](#isUseOcr--) | Возвращает значение, указывающее, используется ли OCR Connector для извлечения текста. |
|
|  | [getOcrOptions()](#getOcrOptions--) | Возвращает дополнительные параметры для функциональности OCR. |
|
|  | [isIncludeAnnotations()](#isIncludeAnnotations--) | Возвращает значение, указывающее, включены ли аннотации в извлечённый текст. |
|
|  | [setIncludeAnnotations(boolean includeAnnotations)](#setIncludeAnnotations-boolean-) | Устанавливает значение, указывающее, включены ли аннотации в извлечённый текст. |
|
### TextOptions(boolean useRawModeIfPossible) {#TextOptions-boolean-}
```
public TextOptions(boolean useRawModeIfPossible)
```


Создаёт новый экземпляр класса [TextOptions](../../com.groupdocs.parser.options/textoptions).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | Значение, указывающее, используется ли необработанный режим. |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr) {#TextOptions-boolean-boolean-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr)
```


Создаёт новый экземпляр класса [TextOptions](../../com.groupdocs.parser.options/textoptions) с опцией использования OCR.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | Значение, указывающее, используется ли необработанный режим. |
|
|  | useOcr | boolean | Значение, указывающее, используется ли функциональность OCR для извлечения текста. |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions) {#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)
```


Создаёт новый экземпляр класса [TextOptions](../../com.groupdocs.parser.options/textoptions) с возможностью задавать параметры OCR.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | Значение, указывающее, используется ли необработанный режим. |
|
|  | useOcr | boolean | Значение, указывающее, используется ли функциональность OCR для извлечения текста. |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Дополнительные параметры для функциональности OCR. |
|

### isUseRawModeIfPossible() {#isUseRawModeIfPossible--}
```
public boolean isUseRawModeIfPossible()
```


Возвращает значение, указывающее, используется ли необработанный режим.


**Returns:**
boolean —  true  если используется необработанный режим; в противном случае  false .

### isUseOcr() {#isUseOcr--}
```
public boolean isUseOcr()
```


Возвращает значение, указывающее, используется ли OCR Connector для извлечения текста.


**Returns:**
boolean —  true  если используется функциональность OCR; в противном случае  false .

### getOcrOptions() {#getOcrOptions--}
```
public OcrOptions getOcrOptions()
```


Возвращает дополнительные параметры для функциональности OCR.


**Returns:**
[OcrOptions](../../com.groupdocs.parser.options/ocroptions) - An instance of [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with the additional OCR options.

### isIncludeAnnotations() {#isIncludeAnnotations--}
```
public boolean isIncludeAnnotations()
```


Возвращает значение, указывающее, включены ли аннотации в извлечённый текст. Значение по умолчанию —  false .


**Returns:**
boolean —  true  если аннотации включены; в противном случае  false .

### setIncludeAnnotations(boolean includeAnnotations) {#setIncludeAnnotations-boolean-}
```
public void setIncludeAnnotations(boolean includeAnnotations)
```


Устанавливает значение, указывающее, включены ли аннотации в извлечённый текст.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | includeAnnotations | boolean | true  для включения аннотаций в извлечённый текст. |
|


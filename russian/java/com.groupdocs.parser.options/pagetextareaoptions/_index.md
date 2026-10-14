---
title: "PageTextAreaOptions"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет параметры, используемые для извлечения областей текста страниц."
type: docs
weight: 32
url: /ru/java/com.groupdocs.parser.options/pagetextareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTextAreaOptions extends PageAreaOptions
```

Предоставляет параметры, используемые для извлечения областей текста страниц.

Экземпляр класса [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) используется в качестве параметра в [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-)
и методы [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-) . См. примеры использования там.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [PageTextAreaOptions()](#PageTextAreaOptions--) | Инициализирует новый экземпляр класса [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) со значениями по умолчанию. |
|
|  | [PageTextAreaOptions(boolean useOcr)](#PageTextAreaOptions-boolean-) | Создаёт новый экземпляр класса [TextOptions](../../com.groupdocs.parser.options/textoptions) с опцией использования OCR. |
|
|  | [PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)](#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-) | Создаёт новый экземпляр класса [TextOptions](../../com.groupdocs.parser.options/textoptions) с возможностью задавать параметры OCR. |
|
|  | [PageTextAreaOptions(String expression)](#PageTextAreaOptions-java.lang.String-) | Инициализирует новый экземпляр класса [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) с регулярным выражением. |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-) | Инициализирует новый экземпляр класса [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) с регулярным выражением и прямоугольной областью. |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-) | Инициализирует новый экземпляр класса [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) с регулярным выражением, прямоугольной областью и размером игнорируемой границы. |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-) | Инициализирует новый экземпляр класса [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions). |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-) | Инициализирует новый экземпляр класса [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) с размером игнорируемой границы. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getExpression()](#getExpression--) | Возвращает регулярное выражение. |
|
|  | [isMatchCase()](#isMatchCase--) | Возвращает значение, что регистр текста не игнорируется. |
|
|  | [isUniteSegments()](#isUniteSegments--) | Возвращает значение, указывающее, объединены ли сегменты. |
|
|  | [isIgnoreFormatting()](#isIgnoreFormatting--) | Возвращает значение, указывающее, игнорируется ли форматирование текста. |
|
|  | [isUseOcr()](#isUseOcr--) | Возвращает значение, указывающее, используется ли OCR Connector для извлечения текста. |
|
|  | [getOcrOptions()](#getOcrOptions--) | Возвращает дополнительные параметры для функциональности OCR. |
|
### PageTextAreaOptions() {#PageTextAreaOptions--}
```
public PageTextAreaOptions()
```


Инициализирует новый экземпляр класса [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) со значениями по умолчанию.


### PageTextAreaOptions(boolean useOcr) {#PageTextAreaOptions-boolean-}
```
public PageTextAreaOptions(boolean useOcr)
```


Создаёт новый экземпляр класса [TextOptions](../../com.groupdocs.parser.options/textoptions) с опцией использования OCR.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | useOcr | boolean | Значение, указывающее, используется ли функциональность OCR для извлечения текста. |
|

### PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions) {#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)
```


Создаёт новый экземпляр класса [TextOptions](../../com.groupdocs.parser.options/textoptions) с возможностью задавать параметры OCR.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | useOcr | boolean | Значение, указывающее, используется ли функциональность OCR для извлечения текста. |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Дополнительные параметры для функциональности OCR. |
|

### PageTextAreaOptions(String expression) {#PageTextAreaOptions-java.lang.String-}
```
public PageTextAreaOptions(String expression)
```


Инициализирует новый экземпляр класса [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) с регулярным выражением. Другие параметры задаются по умолчанию (см. замечания для деталей).

Следующие свойства имеют значения по умолчанию:

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 
* Rectangle:  null 


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | expression | java.lang.String | Регулярное выражение. |
|

### PageTextAreaOptions(String expression, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle)
```


Инициализирует новый экземпляр класса [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) с регулярным выражением и прямоугольной областью. Другие параметры задаются по умолчанию (см. замечания для деталей).

Следующие свойства имеют значения по умолчанию:

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | expression | java.lang.String | Регулярное выражение. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область, содержащая области страниц. |
|

### PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)
```


Инициализирует новый экземпляр класса [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) с регулярным выражением, прямоугольной областью и размером игнорируемой границы. Другие параметры задаются по умолчанию (см. замечания для деталей).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | expression | java.lang.String | Регулярное выражение. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область, содержащая области страниц. |
|
|  | rectangleTolerance | double | Размер границы, игнорируемой при захвате прямоугольной областью. Он измеряется как доля высоты текстового элемента. |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)
```


Инициализирует новый экземпляр класса [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | expression | java.lang.String | Регулярное выражение. |
|
|  | matchCase | boolean | Значение, указывающее, не игнорируется ли регистр текста. |
|
|  | uniteSegments | boolean | Значение, указывающее, объединены ли сегменты. |
|
|  | ignoreFormatting | boolean | Значение, указывающее, игнорируется ли форматирование текста. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область, содержащая области страниц. |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```


Инициализирует новый экземпляр класса [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) с размером игнорируемой границы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | expression | java.lang.String | Регулярное выражение. |
|
|  | matchCase | boolean | Значение, указывающее, не игнорируется ли регистр текста. |
|
|  | uniteSegments | boolean | Значение, указывающее, объединены ли сегменты. |
|
|  | ignoreFormatting | boolean | Значение, указывающее, игнорируется ли форматирование текста. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область, содержащая области страниц. |
|
|  | rectangleTolerance | double | Размер границы, игнорируемой при захвате прямоугольной областью. Он измеряется как доля высоты текстового элемента. |
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

### isUniteSegments() {#isUniteSegments--}
```
public boolean isUniteSegments()
```


Возвращает значение, указывающее, объединены ли сегменты.


**Returns:**
boolean — {code true}, если сегменты объединены; иначе {code false}.

### isIgnoreFormatting() {#isIgnoreFormatting--}
```
public boolean isIgnoreFormatting()
```


Возвращает значение, указывающее, игнорируется ли форматирование текста.


**Returns:**
boolean — true, если форматирование текста игнорируется; иначе false.

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


---
title: "OcrOptions"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет параметры, используемые для OCR Connector."
type: docs
weight: 27
url: /ru/java/com.groupdocs.parser.options/ocroptions/
---
**Inheritance:**
java.lang.Object
```
public class OcrOptions
```

Предоставляет параметры, используемые для OCR Connector.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [OcrOptions()](#OcrOptions--) | Инициализирует новый экземпляр класса [OcrOptions](../../com.groupdocs.parser.options/ocroptions) с значениями по умолчанию. |
|
|  | [OcrOptions(Rectangle rectangle)](#OcrOptions-com.groupdocs.parser.data.Rectangle-) | Инициализирует новый экземпляр класса [OcrOptions](../../com.groupdocs.parser.options/ocroptions) с прямоугольной областью. |
|
|  | [OcrOptions(PagePreviewOptions pagePreviewOptions)](#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-) | Инициализирует новый экземпляр класса [OcrOptions](../../com.groupdocs.parser.options/ocroptions) с параметрами предварительного просмотра страницы. |
|
|  | [OcrOptions(OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-) | Инициализирует новый экземпляр класса [OcrOptions](../../com.groupdocs.parser.options/ocroptions) с объектом [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-) | Инициализирует новый экземпляр класса [OcrOptions](../../com.groupdocs.parser.options/ocroptions) с прямоугольной областью и объектом [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-) | Инициализирует новый экземпляр класса [OcrOptions](../../com.groupdocs.parser.options/ocroptions). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Возвращает прямоугольную область, ограничивающую область страницы, используемую для распознавания текста. |
|
|  | [getHandler()](#getHandler--) | Возвращает обработчик событий для перехвата OCR‑событий. |
|
|  | [getUseSpellChecker()](#getUseSpellChecker--) | Получает значение, указывающее, используется ли проверка орфографии. |
|
|  | [getPagePreviewOptions()](#getPagePreviewOptions--) | Получает параметры предварительного просмотра страницы, используемые для рендеринга страницы, передаваемой в OCR‑движок. |
|
|  | [setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)](#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-) | Устанавливает параметры предварительного просмотра страницы, используемые для рендеринга страницы, передаваемой в OCR‑движок. |
|
|  | [getLanguage()](#getLanguage--) | Получает язык, используемый для оптического распознавания символов. |
|
|  | [setLanguage(Language language)](#setLanguage-com.groupdocs.parser.options.Language-) | Устанавливает язык, используемый для оптического распознавания символов. |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | Устанавливает прямоугольную область, ограничивающую область страницы, используемую для распознавания текста. |
|
|  | [setHandler(OcrEventHandler handler)](#setHandler-com.groupdocs.parser.options.OcrEventHandler-) | Устанавливает обработчик событий для перехвата OCR‑событий. |
|
|  | [setUseSpellChecker(boolean useSpellChecker)](#setUseSpellChecker-boolean-) | Устанавливает значение, указывающее, используется ли проверка орфографии. |
|
### OcrOptions() {#OcrOptions--}
```
public OcrOptions()
```


Инициализирует новый экземпляр класса [OcrOptions](../../com.groupdocs.parser.options/ocroptions) с значениями по умолчанию.


### OcrOptions(Rectangle rectangle) {#OcrOptions-com.groupdocs.parser.data.Rectangle-}
```
public OcrOptions(Rectangle rectangle)
```


Инициализирует новый экземпляр класса [OcrOptions](../../com.groupdocs.parser.options/ocroptions) с прямоугольной областью.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область, ограничивающая область страницы, используемую для распознавания текста. |
|

### OcrOptions(PagePreviewOptions pagePreviewOptions) {#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OcrOptions(PagePreviewOptions pagePreviewOptions)
```


Инициализирует новый экземпляр класса [OcrOptions](../../com.groupdocs.parser.options/ocroptions) с параметрами предварительного просмотра страницы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | Параметры, используемые для рендеринга предварительного просмотра страницы, передаваемой в OCR‑движок. |
|

### OcrOptions(OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(OcrEventHandler handler)
```


Инициализирует новый экземпляр класса [OcrOptions](../../com.groupdocs.parser.options/ocroptions) с объектом [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Экземпляр [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) для перехвата OCR‑событий. |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler)
```


Инициализирует новый экземпляр класса [OcrOptions](../../com.groupdocs.parser.options/ocroptions) с прямоугольной областью и объектом [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область, ограничивающая область страницы, используемую для распознавания текста. |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Экземпляр [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) для перехвата OCR‑событий. |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)
```


Инициализирует новый экземпляр класса [OcrOptions](../../com.groupdocs.parser.options/ocroptions).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область, ограничивающая область страницы, используемую для распознавания текста. |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Экземпляр [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) для перехвата OCR‑событий. |
|
|  | `useSpellCheker` | boolean | Значение, указывающее, используется ли проверка орфографии. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Возвращает прямоугольную область, ограничивающую область страницы, используемую для распознавания текста.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that constraints the page area which is used for text recognizing;  null  if it isn't set.

### getHandler() {#getHandler--}
```
public OcrEventHandler getHandler()
```


Возвращает обработчик событий для перехвата OCR‑событий.


**Returns:**
[OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) - An instance of [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) class which is used to catch OCR events.

### getUseSpellChecker() {#getUseSpellChecker--}
```
public boolean getUseSpellChecker()
```


Получает значение, указывающее, используется ли проверка орфографии.


**Returns:**
boolean —  true  если проверка орфографии используется; иначе  false .

### getPagePreviewOptions() {#getPagePreviewOptions--}
```
public PagePreviewOptions getPagePreviewOptions()
```


Получает параметры предварительного просмотра страницы, используемые для рендеринга страницы, передаваемой в OCR‑движок.


**Returns:**
[PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) - The [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions), or  null  if not set.

### setPagePreviewOptions(PagePreviewOptions pagePreviewOptions) {#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public void setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)
```


Устанавливает параметры предварительного просмотра страницы, используемые для рендеринга страницы, передаваемой в OCR‑движок.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | Параметры предварительного просмотра страницы. |
|

### getLanguage() {#getLanguage--}
```
public Language getLanguage()
```


Получает язык, используемый для оптического распознавания символов.


**Returns:**
[Language](../../com.groupdocs.parser.options/language) - The [Language](../../com.groupdocs.parser.options/language) enum value. Defaults to [Language.Eng](../../com.groupdocs.parser.options/language#Eng).

### setLanguage(Language language) {#setLanguage-com.groupdocs.parser.options.Language-}
```
public void setLanguage(Language language)
```


Устанавливает язык, используемый для оптического распознавания символов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | language | [Language](../../com.groupdocs.parser.options/language) | Значение перечисления [Language](../../com.groupdocs.parser.options/language). |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


Устанавливает прямоугольную область, ограничивающую область страницы, используемую для распознавания текста.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольник или  null  для сканирования всей страницы. |
|

### setHandler(OcrEventHandler handler) {#setHandler-com.groupdocs.parser.options.OcrEventHandler-}
```
public void setHandler(OcrEventHandler handler)
```


Устанавливает обработчик событий для перехвата OCR‑событий.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Обработчик событий. |
|

### setUseSpellChecker(boolean useSpellChecker) {#setUseSpellChecker-boolean-}
```
public void setUseSpellChecker(boolean useSpellChecker)
```


Устанавливает значение, указывающее, используется ли проверка орфографии.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | `useSpellChecker` | boolean | true  для включения проверки орфографии. |
|


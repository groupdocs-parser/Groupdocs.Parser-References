---
title: "OcrOptions"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Инициализирует новый экземпляр класса OcrOptionsgroupdocs.parser.options/ocroptions с прямоугольной областью."
type: docs
weight: 10
url: /ru/net/groupdocs.parser.options/ocroptions/ocroptions/
---

## OcrOptions() {#constructor}

Инициализирует новый экземпляр класса [`OcrOptions`](../../ocroptions) с прямоугольной областью.

```csharp
public OcrOptions()
```

### См. также

* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(PagePreviewOptions) {#constructor_6}

Инициализирует новый экземпляр класса [`OcrOptions`](../../ocroptions) с прямоугольной областью.

```csharp
public OcrOptions(PagePreviewOptions pagePreviewOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pagePreviewOptions | PagePreviewOptions | Экземпляр класса [`PagePreviewOptions`](../pagepreviewoptions), задающий свойства для генерации предварительного просмотра страниц документа. |

### См. также

* class [PagePreviewOptions](../../pagepreviewoptions)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle) {#constructor_1}

Инициализирует новый экземпляр класса [`OcrOptions`](../../ocroptions) с прямоугольной областью.

```csharp
public OcrOptions(Rectangle rectangle)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rectangle | Rectangle | Прямоугольная область, ограничивающая область страницы, используемую для распознавания текста. |

### См. также

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(OcrEventHandler) {#constructor_5}

Инициализирует новый экземпляр класса [`OcrOptions`](../../ocroptions) с объектом [`OcrEventHandler`](../../ocreventhandler).

```csharp
public OcrOptions(OcrEventHandler handler)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| handler | OcrEventHandler | Экземпляр [`OcrEventHandler`](../../ocreventhandler) для перехвата событий OCR. |

### См. также

* class [OcrEventHandler](../../ocreventhandler)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle, OcrEventHandler) {#constructor_2}

Инициализирует новый экземпляр класса [`OcrOptions`](../../ocroptions) с прямоугольной областью и объектом [`OcrEventHandler`](../../ocreventhandler).

```csharp
public OcrOptions(Rectangle rectangle, OcrEventHandler handler)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rectangle | Rectangle | Прямоугольная область, ограничивающая область страницы, используемую для распознавания текста. |
| handler | OcrEventHandler | Экземпляр [`OcrEventHandler`](../../ocreventhandler) для перехвата событий OCR. |

### См. также

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrEventHandler](../../ocreventhandler)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle, OcrEventHandler, PagePreviewOptions, bool) {#constructor_3}

Инициализирует новый экземпляр класса [`OcrOptions`](../../ocroptions).

```csharp
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, 
    PagePreviewOptions pagePreviewOptions, bool useSpellCheker)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rectangle | Rectangle | Прямоугольная область, ограничивающая область страницы, используемую для распознавания текста. |
| handler | OcrEventHandler | Экземпляр [`OcrEventHandler`](../../ocreventhandler) для перехвата событий OCR. |
| pagePreviewOptions | PagePreviewOptions | Экземпляр класса [`PagePreviewOptions`](../pagepreviewoptions), задающий свойства для генерации предварительного просмотра страниц документа. |
| useSpellCheker | Boolean | Значение, указывающее, используется ли проверка орфографии. |

### См. также

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrEventHandler](../../ocreventhandler)
* class [PagePreviewOptions](../../pagepreviewoptions)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle, OcrEventHandler, PagePreviewOptions, bool, Language) {#constructor_4}

Инициализирует новый экземпляр класса [`OcrOptions`](../../ocroptions).

```csharp
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, 
    PagePreviewOptions pagePreviewOptions, bool useSpellCheker, Language language)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rectangle | Rectangle | Прямоугольная область, ограничивающая область страницы, используемую для распознавания текста. |
| handler | OcrEventHandler | Экземпляр [`OcrEventHandler`](../../ocreventhandler) для перехвата событий OCR. |
| pagePreviewOptions | PagePreviewOptions | Экземпляр класса [`PagePreviewOptions`](../pagepreviewoptions), задающий свойства для генерации предварительного просмотра страниц документа. |
| useSpellCheker | Boolean | Значение, указывающее, используется ли проверка орфографии. |
| language | Язык | Язык, используемый для OCR. |

### См. также

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrEventHandler](../../ocreventhandler)
* class [PagePreviewOptions](../../pagepreviewoptions)
* enum [Language](../../language)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->

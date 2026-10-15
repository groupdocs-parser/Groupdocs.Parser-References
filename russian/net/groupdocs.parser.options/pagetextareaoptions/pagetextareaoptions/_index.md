---
title: "PageTextAreaOptions"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Инициализирует новый экземпляр класса PageTextAreaOptionsgroupdocs.parser.options/pagetextareaoptions с опцией использования OCR."
type: docs
weight: 10
url: /ru/net/groupdocs.parser.options/pagetextareaoptions/pagetextareaoptions/
---

## PageTextAreaOptions() {#constructor}

Инициализирует новый экземпляр класса [`PageTextAreaOptions`](../../pagetextareaoptions) с опцией использования OCR.

```csharp
public PageTextAreaOptions()
```

### См. также

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool) {#constructor_1}

Инициализирует новый экземпляр класса [`PageTextAreaOptions`](../../pagetextareaoptions) с опцией использования OCR.

```csharp
public PageTextAreaOptions(bool useOcr)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| useOcr | Boolean | Значение, указывающее, используется ли функция OCR для извлечения текстовых областей. |

### См. также

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool, OcrOptions) {#constructor_2}

Инициализирует новый экземпляр класса [`PageTextAreaOptions`](../../pagetextareaoptions) с возможностью задавать параметры OCR.

```csharp
public PageTextAreaOptions(bool useOcr, OcrOptions ocrOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| useOcr | Boolean | Значение, указывающее, используется ли функция OCR для извлечения текстовых областей. |
| ocrOptions | OcrOptions | Дополнительные параметры для функциональности OCR. |

### См. также

* class [OcrOptions](../../ocroptions)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string) {#constructor_3}

Инициализирует новый экземпляр класса [`PageTextAreaOptions`](../../pagetextareaoptions) с регулярным выражением. Другие параметры задаются по умолчанию (см. примечания для деталей).

```csharp
public PageTextAreaOptions(string expression)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| expression | Строка | Регулярное выражение. |

### Примечания

Следующие свойства имеют значения по умолчанию:

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

**[`Rectangle`](../../pageareaoptions/rectangle)**

`null`

### См. также

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle) {#constructor_6}

Инициализирует новый экземпляр класса [`PageTextAreaOptions`](../../pagetextareaoptions) с регулярным выражением и прямоугольной областью. Другие параметры задаются по умолчанию (см. замечания для деталей).

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| expression | Строка | Регулярное выражение. |
| rectangle | Rectangle | Прямоугольная область, содержащая области страниц. |

### Примечания

Следующие свойства имеют значения по умолчанию:

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

### См. также

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle, double) {#constructor_7}

Инициализирует новый экземпляр класса [`PageTextAreaOptions`](../../pagetextareaoptions) с регулярным выражением, прямоугольной областью и размером игнорируемой границы. Другие параметры задаются по умолчанию (см. замечания для деталей).

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle, double rectangleTolerance)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| expression | Строка | Регулярное выражение. |
| rectangle | Rectangle | Прямоугольная область, содержащая области страниц. |
| rectangleTolerance | Double | Размер границы, игнорируемой при захвате прямоугольной области. Он измеряется как доля высоты текстового элемента. |

### См. также

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle) {#constructor_4}

Инициализирует новый экземпляр класса [`PageTextAreaOptions`](../../pagetextareaoptions).

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| expression | Строка | Регулярное выражение. |
| matchCase | Boolean | Значение, указывающее, не игнорируется ли регистр текста. |
| uniteSegments | Boolean | Значение, указывающее, объединены ли сегменты. |
| ignoreFormatting | Boolean | Значение, указывающее, игнорируется ли форматирование текста. |
| rectangle | Rectangle | Прямоугольная область, содержащая области страниц. |

### См. также

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle, double) {#constructor_5}

Инициализирует новый экземпляр класса [`PageTextAreaOptions`](../../pagetextareaoptions) с размером игнорируемой границы.

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| expression | Строка | Регулярное выражение. |
| matchCase | Boolean | Значение, указывающее, не игнорируется ли регистр текста. |
| uniteSegments | Boolean | Значение, указывающее, объединены ли сегменты. |
| ignoreFormatting | Boolean | Значение, указывающее, игнорируется ли форматирование текста. |
| rectangle | Rectangle | Прямоугольная область, содержащая области страниц. |
| rectangleTolerance | Double | Размер границы, игнорируемой при захвате прямоугольной области. Он измеряется как доля высоты текстового элемента. |

### См. также

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->

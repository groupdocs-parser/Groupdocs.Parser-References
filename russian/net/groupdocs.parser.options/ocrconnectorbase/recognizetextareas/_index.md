---
title: "RecognizeTextAreas"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Распознавать текстовые области из потока imageStream."
type: docs
weight: 40
url: /ru/net/groupdocs.parser.options/ocrconnectorbase/recognizetextareas/
---

## RecognizeTextAreas(Stream, Page, OcrOptions) {#recognizetextareas}

Распознать области текста из потока *imageStream*.

```csharp
public virtual IList<PageTextArea> RecognizeTextAreas(Stream imageStream, Page page, 
    OcrOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| imageStream | Stream | Изображение, представляющее страницу документа. |
| page | Page | Страница документа. |
| options | OcrOptions | Параметры OCR. |

### Возвращаемое значение

Коллекция объектов [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea); `null`, если распознавание текстовых областей не поддерживается.

### См. также

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Page](../../../groupdocs.parser.data/page)
* class [OcrOptions](../../ocroptions)
* class [OcrConnectorBase](../../ocrconnectorbase)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## RecognizeTextAreas(Stream, IEnumerable&lt;Rectangle&gt;, string, Page, OcrOptions) {#recognizetextareas_3}

Распознать области текста из потока *imageStream*.

```csharp
public virtual IList<PageTextArea> RecognizeTextAreas(Stream imageStream, 
    IEnumerable<Rectangle> rectangles, string allowedSymbols, Page page, OcrOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| imageStream | Stream | Изображение, представляющее страницу документа. |
| rectangles | IEnumerable`1 | Коллекция прямоугольных областей, ограничивающих функциональность OCR. |
| allowedSymbols | Строка | Фильтр разрешённых символов OCR. |
| page | Page | Страница документа. |
| options | OcrOptions | Параметры OCR. |

### Возвращаемое значение

Коллекция объектов [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea); `null`, если распознавание текстовых областей не поддерживается.

### См. также

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [Page](../../../groupdocs.parser.data/page)
* class [OcrOptions](../../ocroptions)
* class [OcrConnectorBase](../../ocrconnectorbase)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->

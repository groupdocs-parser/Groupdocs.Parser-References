---
title: "OcrConnectorBase"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Предоставляет функциональность OCR."
type: docs
weight: 430
url: /ru/net/groupdocs.parser.options/ocrconnectorbase/
---

## OcrConnectorBase class

Предоставляет функциональность OCR.

```csharp
public abstract class OcrConnectorBase
```

## Свойства

| Имя | Описание |
| --- | --- |
| virtual [IsTextAreasSupported](../../groupdocs.parser.options/ocrconnectorbase/istextareassupported) { get; } | Получает значение, указывающее, поддерживается ли извлечение областей текста. |
| virtual [IsTextSupported](../../groupdocs.parser.options/ocrconnectorbase/istextsupported) { get; } | Получает значение, указывающее, поддерживается ли извлечение текста. |

## Методы

| Имя | Описание |
| --- | --- |
| virtual [RecognizeText](../../groupdocs.parser.options/ocrconnectorbase/recognizetext#recognizetext)(Stream, OcrOptions) | Распознать текст из потока *imageStream*. |
| virtual [RecognizeTextAreas](../../groupdocs.parser.options/ocrconnectorbase/recognizetextareas#recognizetextareas)(Stream, Page, OcrOptions) | Распознать области текста из потока *imageStream*. |
| virtual [RecognizeTextAreas](../../groupdocs.parser.options/ocrconnectorbase/recognizetextareas#recognizetextareas_3)(Stream, IEnumerable&lt;Rectangle&gt;, string, Page, OcrOptions) | Распознать области текста из потока *imageStream*. |

### См. также

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->

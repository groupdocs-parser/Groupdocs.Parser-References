---
title: "RecognizeText"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Распознать текст из потока imageStream."
type: docs
weight: 30
url: /ru/net/groupdocs.parser.options/ocrconnectorbase/recognizetext/
---

## OcrConnectorBase.RecognizeText method

Распознать текст из потока *imageStream*.

```csharp
public virtual string RecognizeText(Stream imageStream, OcrOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| imageStream | Stream | Изображение, представляющее страницу документа. |
| options | OcrOptions | Параметры OCR. |

### Возвращаемое значение

Строка, представляющая распознанный текст; `null`, если распознавание текста не поддерживается.

### См. также

* class [OcrOptions](../../ocroptions)
* class [OcrConnectorBase](../../ocrconnectorbase)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->

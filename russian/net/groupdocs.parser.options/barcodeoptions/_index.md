---
title: "BarcodeOptions"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Предоставляет параметры, которые используются для извлечения штрих‑кода."
type: docs
weight: 200
url: /ru/net/groupdocs.parser.options/barcodeoptions/
---

## BarcodeOptions class

Предоставляет параметры, которые используются для извлечения штрих‑кода.

```csharp
public sealed class BarcodeOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [BarcodeOptions](barcodeoptions#constructor)() | Инициализирует новый экземпляр класса [`BarcodeOptions`](../barcodeoptions) со значениями по умолчанию. |
| [BarcodeOptions](barcodeoptions#constructor_1)(Rectangle) | Инициализирует новый экземпляр класса [`BarcodeOptions`](../barcodeoptions) с прямоугольной областью. |
| [BarcodeOptions](barcodeoptions#constructor_3)(QualityMode, QualityMode, params string[]) | Инициализирует новый экземпляр класса [`BarcodeOptions`](../barcodeoptions) с настройками качества и типами кодов. |
| [BarcodeOptions](barcodeoptions#constructor_2)(Rectangle, QualityMode, QualityMode, float?, bool, params string[]) | Инициализирует новый экземпляр класса [`BarcodeOptions`](../barcodeoptions). |

## Свойства

| Имя | Описание |
| --- | --- |
| [AllowIncorrectBarcodes](../../groupdocs.parser.options/barcodeoptions/allowincorrectbarcodes) { get; set; } | Возвращает значение, указывающее, допускаются ли некорректные штрихкоды. |
| [BarcodeQuality](../../groupdocs.parser.options/barcodeoptions/barcodequality) { get; set; } | Возвращает качество исходного штрихкода. |
| [CodeTypes](../../groupdocs.parser.options/barcodeoptions/codetypes) { get; set; } | Возвращает типы штрихкодов для чтения. |
| [Dimension](../../groupdocs.parser.options/barcodeoptions/dimension) { get; set; } | Возвращает минимальный размер минимального элемента штрихкода. |
| [ImageQuality](../../groupdocs.parser.options/barcodeoptions/imagequality) { get; set; } | Возвращает качество исходного изображения. |
| [PagePreviewOptions](../../groupdocs.parser.options/barcodeoptions/pagepreviewoptions) { get; set; } | Получает или задает параметры предварительного просмотра страниц документа. |
| [Rectangle](../../groupdocs.parser.options/barcodeoptions/rectangle) { get; set; } | Получает прямоугольную область, содержащую области страниц. |

### См. также

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->

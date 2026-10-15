---
title: "PreviewOptions"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Предоставляет параметры для установки требований и делегатов потоков при генерации предварительного просмотра."
type: docs
weight: 550
url: /ru/net/groupdocs.parser.options/previewoptions/
---

## PreviewOptions class

Предоставляет параметры для установки требований и делегатов потоков при генерации предварительного просмотра.

```csharp
public class PreviewOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PreviewOptions](previewoptions#constructor)(CreatePageStream) | Инициализирует новый экземпляр класса [`PreviewOptions`](../previewoptions), вызывая закрытие выходного потока. |
| [PreviewOptions](previewoptions#constructor_1)(CreatePageStream, ReleasePageStream) | Инициализирует новый экземпляр класса [`PreviewOptions`](../previewoptions), вызывая возврат выходного потока клиенту для дальнейшего использования. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CreatePageStream](../../groupdocs.parser.options/previewoptions/createpagestream) { get; set; } | Получает или задает экземпляр делегата создания потока страницы. |
| [Dpi](../../groupdocs.parser.options/previewoptions/dpi) { get; set; } | Получает или задает значение dpi. |
| [Height](../../groupdocs.parser.options/previewoptions/height) { get; set; } | Получает или задает высоту предварительного просмотра страницы. |
| [PageNumbers](../../groupdocs.parser.options/previewoptions/pagenumbers) { get; set; } | Получает или задает массив номеров страниц для генерации предварительных просмотров. |
| [PreviewFormat](../../groupdocs.parser.options/previewoptions/previewformat) { get; set; } | Получает или задает формат изображения предварительного просмотра. |
| [PreviewPageRender](../../groupdocs.parser.options/previewoptions/previewpagerender) { get; set; } | Получает или задает экземпляр делегата информации о рендеринге предварительного просмотра страницы. |
| [ReleasePageStream](../../groupdocs.parser.options/previewoptions/releasepagestream) { get; set; } | Получает или задает экземпляр делегата завершения предварительного просмотра страницы. |
| [Width](../../groupdocs.parser.options/previewoptions/width) { get; set; } | Получает или задает ширину предварительного просмотра страницы. |

### См. также

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->

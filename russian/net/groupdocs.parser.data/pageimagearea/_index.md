---
title: "PageImageArea"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Представляет область изображения на странице, используемую для представления изображения на странице в функции парсинга по шаблону или вложения изображения, если изображения извлекаются из электронных писем или ZIP‑архивов."
type: docs
weight: 830
url: /ru/net/groupdocs.parser.data/pageimagearea/
---

## PageImageArea class

Представляет область изображения на странице, используемую для представления изображения на странице в функции парсинга по шаблону или вложения изображения, если изображения извлекаются из электронных писем или ZIP‑архивов.

```csharp
public sealed class PageImageArea : PageArea
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PageImageArea](pageimagearea#constructor)(Stream, FileType, double) | Инициализирует новый экземпляр класса [`PageImageArea`](../pageimagearea). |
| [PageImageArea](pageimagearea#constructor_1)(Stream, FileType, double, Page, Rectangle) | Инициализирует новый экземпляр класса [`PageImageArea`](../pageimagearea). |

## Свойства

| Имя | Описание |
| --- | --- |
| [FileType](../../groupdocs.parser.data/pageimagearea/filetype) { get; } | Возвращает формат изображения. |
| [Page](../../groupdocs.parser.data/pagearea/page) { get; } | Возвращает информацию о странице документа, такую как индекс страницы и её размер. |
| [Rectangle](../../groupdocs.parser.data/pagearea/rectangle) { get; } | Получает прямоугольную область. |
| [Rotation](../../groupdocs.parser.data/pageimagearea/rotation) { get; } | Получает угол поворота изображения. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetImageStream](../../groupdocs.parser.data/pageimagearea/getimagestream#getimagestream)() | Возвращает поток изображения. |
| [GetImageStream](../../groupdocs.parser.data/pageimagearea/getimagestream#getimagestream_1)(ImageOptions) | Возвращает поток изображения в другом формате. |
| [Save](../../groupdocs.parser.data/pageimagearea/save#save)(string) | Сохраняет изображение в файл. |
| [Save](../../groupdocs.parser.data/pageimagearea/save#save_1)(string, ImageOptions) | Сохраняет изображение в файл в другом формате. |

### Примечания

Экземпляр класса [`PageImageArea`](../pageimagearea) используется в качестве возвращаемого значения следующих методов:

* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetImages`](../../groupdocs.parser/parser/getimages)

Смотрите примеры использования там.

### См. также

* class [PageArea](../pagearea)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->

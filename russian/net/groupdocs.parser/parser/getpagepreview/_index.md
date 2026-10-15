---
title: "GetPagePreview"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Создаёт предварительный просмотр страницы документа."
type: docs
weight: 150
url: /ru/net/groupdocs.parser/parser/getpagepreview/
---

## GetPagePreview(int) {#getpagepreview}

Создаёт предварительный просмотр страницы документа.

```csharp
public Stream GetPagePreview(int pageIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Нулевой индекс страницы. |

### Возвращаемое значение

Экземпляр Stream, содержащий изображение страницы документа; `null`, если генерация предварительного просмотра страницы не поддерживается.

### См. также

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetPagePreview(int, PagePreviewOptions) {#getpagepreview_1}

Создаёт предварительный просмотр страницы документа с использованием параметров настройки.

```csharp
public Stream GetPagePreview(int pageIndex, PagePreviewOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Нулевой индекс страницы. |
| options | PagePreviewOptions | Параметры для настройки генерации предварительного просмотра. |

### Возвращаемое значение

Экземпляр Stream, содержащий изображение страницы документа; `null`, если генерация предварительного просмотра страницы не поддерживается.

### См. также

* class [PagePreviewOptions](../../../groupdocs.parser.options/pagepreviewoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->

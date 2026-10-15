---
title: "PreviewOptions"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Инициализирует новый экземпляр класса PreviewOptionsgroupdocs.parser.options/previewoptions, вызывая закрытие выходного потока."
type: docs
weight: 10
url: /ru/net/groupdocs.parser.options/previewoptions/previewoptions/
---

## PreviewOptions(CreatePageStream) {#constructor}

Инициализирует новый экземпляр класса [`PreviewOptions`](../../previewoptions), вызывая закрытие выходного потока.

```csharp
public PreviewOptions(CreatePageStream createPageStream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| createPageStream | CreatePageStream | Создаёт поток для предварительного просмотра конкретной страницы. |

### См. также

* delegate [CreatePageStream](../../createpagestream)
* class [PreviewOptions](../../previewoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PreviewOptions(CreatePageStream, ReleasePageStream) {#constructor_1}

Инициализирует новый экземпляр класса [`PreviewOptions`](../../previewoptions), вызывая возврат выходного потока клиенту для дальнейшего использования.

```csharp
public PreviewOptions(CreatePageStream createPageStream, ReleasePageStream releasePageStream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| createPageStream | CreatePageStream | Создаёт поток для предварительного просмотра конкретной страницы |
| releasePageStream | ReleasePageStream | Уведомляет о завершении генерации предварительного просмотра страницы и получает выходной поток. |

### См. также

* delegate [CreatePageStream](../../createpagestream)
* delegate [ReleasePageStream](../../releasepagestream)
* class [PreviewOptions](../../previewoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->

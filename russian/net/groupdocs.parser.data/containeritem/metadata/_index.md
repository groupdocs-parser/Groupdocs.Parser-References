---
title: "Metadata"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Получает коллекцию элементов метаданных."
type: docs
weight: 30
url: /ru/net/groupdocs.parser.data/containeritem/metadata/
---

## ContainerItem.Metadata property

Получает коллекцию элементов метаданных.

```csharp
public IEnumerable<MetadataItem> Metadata { get; }
```

### Property Value

Коллекция объектов [`MetadataItem`](../../metadataitem); пустая, если метаданные не заданы.

### Примечания

Эти метаданные относятся к самому элементу контейнера, а не к документу. В зависимости от типа контейнера метаданные могут содержать следующие элементы:

**Email Attachments**

**Name**

**Description**

**content-type**

MIME‑тип содержимого вложения.

**ZIP Archives**

**Name**

**Description**

**date**

Время и дата последнего изменения файла, указанного в Zip‑записи.

**disposition**

Для определения, является ли вложение изображения встроенным, используется метаданные 'disposition'. Если они присутствуют, они могут принимать значения 'inline' или 'attachment'.

**Outlook Storage**

**Name**

**Description**

**date**

Время и дата последнего изменения элемента Outlook Storage.

**email-sender**

Значение поля "sender".

**email-to**

Значение поля "to".

**subject**

Значение поля "subject".

### См. также

* class [MetadataItem](../../metadataitem)
* class [ContainerItem](../../containeritem)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->

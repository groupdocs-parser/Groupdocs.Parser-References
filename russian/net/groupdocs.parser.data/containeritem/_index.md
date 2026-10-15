---
title: "ContainerItem"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Представляет элемент контейнера, такой как объект Zip‑архива, вложение электронной почты, элемент PDF Portfolio и т.п."
type: docs
weight: 720
url: /ru/net/groupdocs.parser.data/containeritem/
---

## ContainerItem class

Представляет элемент контейнера, такой как объект Zip‑архива, вложение электронной почты, элемент PDF‑портфолио и т.д.

```csharp
public sealed class ContainerItem
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Directory](../../groupdocs.parser.data/containeritem/directory) { get; } | Получает каталог элемента. |
| [FilePath](../../groupdocs.parser.data/containeritem/filepath) { get; } | Получает полный путь к элементу. |
| [Metadata](../../groupdocs.parser.data/containeritem/metadata) { get; } | Получает коллекцию элементов метаданных. |
| [Name](../../groupdocs.parser.data/containeritem/name) { get; } | Получает имя элемента. |
| [Size](../../groupdocs.parser.data/containeritem/size) { get; } | Получает размер элемента. |

## Методы

| Имя | Описание |
| --- | --- |
| [DetectFileType](../../groupdocs.parser.data/containeritem/detectfiletype)(FileTypeDetectionMode) | Определяет тип файла элемента контейнера. |
| [GetMetadataValue](../../groupdocs.parser.data/containeritem/getmetadatavalue)(string) | Получает значение метаданных. |
| [OpenParser](../../groupdocs.parser.data/containeritem/openparser#openparser)() | Создаёт объект [`Parser`](../../groupdocs.parser/parser) для содержимого элемента. |
| [OpenParser](../../groupdocs.parser.data/containeritem/openparser#openparser_1)(LoadOptions) | Создаёт объект [`Parser`](../../groupdocs.parser/parser) для содержимого элемента с [`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [OpenParser](../../groupdocs.parser.data/containeritem/openparser#openparser_2)(LoadOptions, ParserSettings) | Создаёт объект [`Parser`](../../groupdocs.parser/parser) для содержимого элемента с [`LoadOptions`](../../groupdocs.parser.options/loadoptions) и [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [OpenStream](../../groupdocs.parser.data/containeritem/openstream)() | Открывает поток содержимого элемента. |

### Примечания

Экземпляр класса [`ContainerItem`](../containeritem) используется в качестве возвращаемого значения метода [`GetContainer`](../../groupdocs.parser/parser/getcontainer). См. примеры использования там.

### См. также

* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->

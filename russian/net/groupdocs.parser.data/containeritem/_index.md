---
title: ContainerItem
second_title: Справочник по API GroupDocs.Parser для .NET
description: Представляет элемент контейнера такой как объект Zipархива вложение электронной почты элемент портфолио PDF и т. д.
type: docs
weight: 10
url: /ru/net/groupdocs.parser.data/containeritem/
---
## ContainerItem class

Представляет элемент контейнера, такой как объект Zip-архива, вложение электронной почты, элемент портфолио PDF и т. д.

```csharp
public sealed class ContainerItem
```

## Характеристики

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
| [OpenParser](../../groupdocs.parser.data/containeritem/openparser#openparser)() | Создает[`Parser`](../../groupdocs.parser/parser) объект для содержимого элемента. |
| [OpenParser](../../groupdocs.parser.data/containeritem/openparser#openparser_1)(LoadOptions) | Создает[`Parser`](../../groupdocs.parser/parser) объект для содержимого элемента с[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [OpenParser](../../groupdocs.parser.data/containeritem/openparser#openparser_2)(LoadOptions, ParserSettings) | Создает[`Parser`](../../groupdocs.parser/parser) объект для содержимого элемента с[`LoadOptions`](../../groupdocs.parser.options/loadoptions) и[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [OpenStream](../../groupdocs.parser.data/containeritem/openstream)() | Открывает поток содержимого элемента. |

### Примечания

Экземпляр[`ContainerItem`](../containeritem) класс используется как возвращаемое значение из[`GetContainer`](../../groupdocs.parser/parser/getcontainer) метод. См. примеры использования там.

### Смотрите также

* пространство имен [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* сборка [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

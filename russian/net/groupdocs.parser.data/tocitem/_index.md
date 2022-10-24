---
title: TocItem
second_title: Справочник по API GroupDocs.Parser для .NET
description: Представляет элемент который используется в функции извлечения оглавления.
type: docs
weight: 200
url: /ru/net/groupdocs.parser.data/tocitem/
---
## TocItem class

Представляет элемент, который используется в функции извлечения оглавления.

```csharp
public class TocItem
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [TocItem](tocitem)(int, string, int?) | Инициализирует новый экземпляр[`TocItem`](../tocitem) класс. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [Depth](../../groupdocs.parser.data/tocitem/depth) { get; } | Получает уровень глубины. |
| [PageIndex](../../groupdocs.parser.data/tocitem/pageindex) { get; } | Получает индекс страницы. |
| [Text](../../groupdocs.parser.data/tocitem/text) { get; } | Получает текст. |

## Методы

| Имя | Описание |
| --- | --- |
| virtual [ExtractText](../../groupdocs.parser.data/tocitem/extracttext)() | Извлекает текст из документа, к которому[`TocItem`](../tocitem) объект ссылается. |

### Примечания

Экземпляр[`TocItem`](../tocitem) класс используется как возвращаемое значение из[`GetToc`](../../groupdocs.parser/parser/gettoc) методы. См. примеры использования там.

### Смотрите также

* пространство имен [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* сборка [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
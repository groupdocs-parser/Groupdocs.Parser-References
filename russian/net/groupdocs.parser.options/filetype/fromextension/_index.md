---
title: "FromExtension"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Сопоставляет расширение файла с типом файла."
type: docs
weight: 930
url: /ru/net/groupdocs.parser.options/filetype/fromextension/
---

## FileType.FromExtension method

Сопоставляет расширение файла с типом файла.

```csharp
public static FileType FromExtension(string extension)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| extension | Строка | Расширение файла (включая точку "."). |

### Возвращаемое значение

Если тип файла поддерживается, возвращает его, иначе возвращает тип файла по умолчанию [`Unknown`](../unknown).

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | Выбрасывается, когда *extension* имеет значение null или пустую строку. |

### См. также

* class [FileType](../../filetype)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->

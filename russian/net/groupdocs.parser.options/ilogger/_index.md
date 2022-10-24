---
title: ILogger
second_title: Справочник по API GroupDocs.Parser для .NET
description: Определяет интерфейс регистратора который используется для регистрации событий и ошибок при извлечении данных.
type: docs
weight: 420
url: /ru/net/groupdocs.parser.options/ilogger/
---
## ILogger interface

Определяет интерфейс регистратора, который используется для регистрации событий и ошибок при извлечении данных.

```csharp
public interface ILogger
```

## Методы

| Имя | Описание |
| --- | --- |
| [Error](../../groupdocs.parser.options/ilogger/error)(string, Exception) | Регистрирует ошибку, возникшую при извлечении данных. |
| [Trace](../../groupdocs.parser.options/ilogger/trace)(string) | Регистрирует событие, произошедшее во время извлечения данных. |
| [Warning](../../groupdocs.parser.options/ilogger/warning)(string) | Регистрирует предупреждение, возникшее во время извлечения данных. |

### Примечания

**Учить больше:**

* [логирование](https://docs.groupdocs.com/display/parsernet/Logging)

### Смотрите также

* пространство имен [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* сборка [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
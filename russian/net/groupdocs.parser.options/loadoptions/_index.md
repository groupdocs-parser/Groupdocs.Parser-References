---
title: "LoadOptions"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Предоставляет параметры, которые используются для открытия файла."
type: docs
weight: 420
url: /ru/net/groupdocs.parser.options/loadoptions/
---

## LoadOptions class

Предоставляет параметры, которые используются для открытия файла.

```csharp
public sealed class LoadOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [LoadOptions](loadoptions#constructor)() | Инициализирует новый экземпляр класса [`LoadOptions`](../loadoptions) с пустым [`Password`](./password), [`FileFormat`](./fileformat), равным Unknown, и кодировками по умолчанию. |
| [LoadOptions](loadoptions#constructor_1)(FileFormat) | Инициализирует новый экземпляр класса [`LoadOptions`](../loadoptions) с пустым [`Password`](./password) и кодировками по умолчанию. |
| [LoadOptions](loadoptions#constructor_5)(FileType) | Инициализирует новый экземпляр класса [`LoadOptions`](../loadoptions) с пустым [`Password`](./password) и кодировками по умолчанию. |
| [LoadOptions](loadoptions#constructor_9)(string) | Инициализирует новый экземпляр класса [`LoadOptions`](../loadoptions) с [`FileFormat`](./fileformat), равным Unknown, и кодировками по умолчанию. |
| [LoadOptions](loadoptions#constructor_10)(TimeSpan) | Инициализирует новый экземпляр класса [`LoadOptions`](../loadoptions) с *timeout*. |
| [LoadOptions](loadoptions#constructor_2)(FileFormat, string) | Инициализирует новый экземпляр класса [`LoadOptions`](../loadoptions) с паролем и кодировками по умолчанию. |
| [LoadOptions](loadoptions#constructor_6)(FileType, string) | Инициализирует новый экземпляр класса [`LoadOptions`](../loadoptions) с паролем и кодировками по умолчанию. |
| [LoadOptions](loadoptions#constructor_3)(FileFormat, string, Encoding, Encoding) | Инициализирует новый экземпляр класса [`LoadOptions`](../loadoptions) с пользовательскими кодировками. |
| [LoadOptions](loadoptions#constructor_7)(FileType, string, Encoding, Encoding) | Инициализирует новый экземпляр класса [`LoadOptions`](../loadoptions) с пользовательскими кодировками. |
| [LoadOptions](loadoptions#constructor_4)(FileFormat, string, Encoding, Encoding, TimeSpan) | Инициализирует новый экземпляр полностью настроенного класса [`LoadOptions`](../loadoptions). |
| [LoadOptions](loadoptions#constructor_8)(FileType, string, Encoding, Encoding, TimeSpan) | Инициализирует новый экземпляр полностью настроенного класса [`LoadOptions`](../loadoptions). |

## Свойства

| Имя | Описание |
| --- | --- |
| [DefaultAnsiEncoding](../../groupdocs.parser.options/loadoptions/defaultansiencoding) { get; } | Получает кодировку ANSI по умолчанию, используемую для обнаружения кодировки. |
| [Encoding](../../groupdocs.parser.options/loadoptions/encoding) { get; } | Получает кодировку документа. |
| [FileFormat](../../groupdocs.parser.options/loadoptions/fileformat) { get; } | Получает формат файла. |
| [FileType](../../groupdocs.parser.options/loadoptions/filetype) { get; } | Получает тип файла. |
| [Password](../../groupdocs.parser.options/loadoptions/password) { get; } | Получает пароль. |
| [Timeout](../../groupdocs.parser.options/loadoptions/timeout) { get; } | Получает значение, представляющее количество миллисекунд ожидания. |

### Примечания

Экземпляр этого класса используется в качестве параметра в конструкторах класса [`Parser`](../../groupdocs.parser/parser):

* [`Parser`](../../groupdocs.parser/parser/parser)
* [`Parser`](../../groupdocs.parser/parser/parser)

Смотрите примеры использования там.

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)

### См. также

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->

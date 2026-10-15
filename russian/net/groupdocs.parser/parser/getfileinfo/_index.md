---
title: "GetFileInfo"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Возвращает общую информацию о файле."
type: docs
weight: 260
url: /ru/net/groupdocs.parser/parser/getfileinfo/
---

## GetFileInfo(string) {#getfileinfo_2}

Возвращает общую информацию о файле.

```csharp
public static FileInfo GetFileInfo(string filePath)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | Строка | Путь к файлу. |

### Возвращаемое значение

Экземпляр класса [`FileInfo`](../../../groupdocs.parser.options/fileinfo).

### Примеры

Следующий код показывает, как проверить, защищён ли файл паролем:

```csharp
// Получить информацию о файле
Options.FileInfo info = Parser.GetFileInfo(filePath);
// Проверьте свойство IsEncrypted
Console.WriteLine(info.IsEncrypted ? "Password is required" : "");
```

### См. также

* class [FileInfo](../../../groupdocs.parser.options/fileinfo)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetFileInfo(string, LoadOptions) {#getfileinfo_3}

Возвращает общую информацию о файле.

```csharp
public static FileInfo GetFileInfo(string filePath, LoadOptions loadOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | Строка | Путь к файлу. |
| loadOptions | LoadOptions | Параметры открытия файла. |

### Возвращаемое значение

Экземпляр класса [`FileInfo`](../../../groupdocs.parser.options/fileinfo).

### Примеры

Следующий код показывает, как проверить тип файла защищённого паролем документа:

```csharp
// Получить информацию о файле
Options.FileInfo info = Parser.GetFileInfo(filePath, new LoadOptions("password"));
// Проверьте свойство IsEncrypted
Console.WriteLine(info.IsEncrypted ? "Password is required" : "");
// Вывести тип файла
Console.WriteLine(info.FileType.ToString());
```

### См. также

* class [FileInfo](../../../groupdocs.parser.options/fileinfo)
* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetFileInfo(Stream) {#getfileinfo}

Возвращает общую информацию о файле.

```csharp
public static FileInfo GetFileInfo(Stream document)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| документ | Stream | Исходный входной поток. |

### Возвращаемое значение

Экземпляр класса [`FileInfo`](../../../groupdocs.parser.options/fileinfo).

### Примеры

Следующий код показывает, как проверить, защищён ли файл паролем:

```csharp
// Получить информацию о файле
Options.FileInfo info = Parser.GetFileInfo(document);
// Проверьте свойство IsEncrypted
Console.WriteLine(info.IsEncrypted ? "Password is required" : "");
```

### См. также

* class [FileInfo](../../../groupdocs.parser.options/fileinfo)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetFileInfo(Stream, LoadOptions) {#getfileinfo_1}

Возвращает общую информацию о файле.

```csharp
public static FileInfo GetFileInfo(Stream document, LoadOptions loadOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| документ | Stream | Исходный входной поток. |
| loadOptions | LoadOptions | Параметры открытия файла. |

### Возвращаемое значение

Экземпляр класса [`FileInfo`](../../../groupdocs.parser.options/fileinfo).

### Примеры

Следующий код показывает, как проверить тип файла защищённого паролем документа:

```csharp
// Получить информацию о файле
Options.FileInfo info = Parser.GetFileInfo(document);
// Проверьте свойство IsEncrypted
Console.WriteLine(info.IsEncrypted ? "Password is required" : "");
// Вывести тип файла
Console.WriteLine(info.FileType.ToString());
```

### См. также

* class [FileInfo](../../../groupdocs.parser.options/fileinfo)
* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->

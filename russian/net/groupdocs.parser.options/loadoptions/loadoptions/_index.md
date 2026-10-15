---
title: "LoadOptions"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Инициализирует новый экземпляр класса LoadOptionsgroupdocs.parser.options/loadoptions с пустым Passwordgroupdocs.parser.options/loadoptions/password, FileFormatgroupdocs.parser.options/loadoptions/fileformat, равным Unknown, и кодировками по умолчанию."
type: docs
weight: 10
url: /ru/net/groupdocs.parser.options/loadoptions/loadoptions/
---

## LoadOptions() {#constructor}

Инициализирует новый экземпляр класса [`LoadOptions`](../../loadoptions) с пустым [`Password`](../password), [`FileFormat`](../fileformat), равным Unknown, и кодировками по умолчанию.

```csharp
public LoadOptions()
```

### См. также

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(TimeSpan) {#constructor_10}

Инициализирует новый экземпляр класса [`LoadOptions`](../../loadoptions) с *timeout*.

```csharp
public LoadOptions(TimeSpan timeout)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| timeout | TimeSpan | TimeSpan, представляющий количество миллисекунд, которое следует ждать. |

### См. также

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(string) {#constructor_9}

Инициализирует новый экземпляр класса [`LoadOptions`](../../loadoptions) с [`FileFormat`](../fileformat), равным Unknown, и кодировками по умолчанию.

```csharp
public LoadOptions(string password)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| password | Строка | Пароль для открытия защищённого паролем файла. |

### См. также

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat) {#constructor_1}

Инициализирует новый экземпляр класса [`LoadOptions`](../../loadoptions) с пустым [`Password`](../password) и кодировками по умолчанию.

```csharp
public LoadOptions(FileFormat fileFormat)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileFormat | FileFormat | Формат файла. |

### См. также

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string) {#constructor_2}

Инициализирует новый экземпляр класса [`LoadOptions`](../../loadoptions) с паролем и кодировками по умолчанию.

```csharp
public LoadOptions(FileFormat fileFormat, string password)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileFormat | FileFormat | Формат файла. |
| password | Строка | Пароль для открытия защищённого паролем файла. |

### См. также

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding) {#constructor_3}

Инициализирует новый экземпляр класса [`LoadOptions`](../../loadoptions) с пользовательскими кодировками.

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileFormat | FileFormat | Формат файла. |
| password | Строка | Пароль для открытия защищённого паролем файла. |
| кодировка | Encoding | Кодировка документа. |
| defaultAnsiEncoding | Encoding | Кодировка ANSI по умолчанию, используемая для определения кодировки. |

### См. также

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding, TimeSpan) {#constructor_4}

Инициализирует новый полностью настроенный экземпляр класса [`LoadOptions`](../../loadoptions).

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileFormat | FileFormat | Формат файла. |
| password | Строка | Пароль для открытия защищённого паролем файла. |
| кодировка | Encoding | Кодировка документа. |
| defaultAnsiEncoding | Encoding | Кодировка ANSI по умолчанию, используемая для определения кодировки. |
| timeout | TimeSpan | TimeSpan, представляющий количество миллисекунд, которое следует ждать. |

### См. также

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType) {#constructor_5}

Инициализирует новый экземпляр класса [`LoadOptions`](../../loadoptions) с пустым [`Password`](../password) и кодировками по умолчанию.

```csharp
public LoadOptions(FileType fileType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileType | FileType | Тип файла. |

### См. также

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string) {#constructor_6}

Инициализирует новый экземпляр класса [`LoadOptions`](../../loadoptions) с паролем и кодировками по умолчанию.

```csharp
public LoadOptions(FileType fileType, string password)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileType | FileType | Тип файла. |
| password | Строка | Пароль для открытия защищённого паролем файла. |

### См. также

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding) {#constructor_7}

Инициализирует новый экземпляр класса [`LoadOptions`](../../loadoptions) с пользовательскими кодировками.

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileType | FileType | Тип файла. |
| password | Строка | Пароль для открытия защищённого паролем файла. |
| кодировка | Encoding | Кодировка документа. |
| defaultAnsiEncoding | Encoding | Кодировка ANSI по умолчанию, используемая для определения кодировки. |

### См. также

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding, TimeSpan) {#constructor_8}

Инициализирует новый полностью настроенный экземпляр класса [`LoadOptions`](../../loadoptions).

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileType | FileType | Тип файла. |
| password | Строка | Пароль для открытия защищённого паролем файла. |
| кодировка | Encoding | Кодировка документа. |
| defaultAnsiEncoding | Encoding | Кодировка ANSI по умолчанию, используемая для определения кодировки. |
| timeout | TimeSpan | TimeSpan, представляющий количество миллисекунд, которое следует ждать. |

### См. также

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->

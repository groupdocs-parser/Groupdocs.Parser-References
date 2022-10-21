---
title: Parser
second_title: Справочник по API GroupDocs.Parser для .NET
description: Инициализирует новый экземплярParsergroupdocs.parser/parser класс для извлечения данных из базы данных.
type: docs
weight: 10
url: /ru/net/groupdocs.parser/parser/parser/
---
## Parser(DbConnection) {#constructor_2}

Инициализирует новый экземпляр[`Parser`](../../parser) класс для извлечения данных из базы данных.

```csharp
public Parser(DbConnection connection)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| connection | DbConnection | Подключение к базе данных. |

### Примечания

**Учить больше:**

* [Извлекать данные из баз данных](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### Примеры

В следующем примере показано, как извлечь данные из базы данных Sqlite:

```csharp
// Создаем объект DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Создаем экземпляр класса Parser для извлечения таблиц из базы данных
using (Parser parser = new Parser(connection))
{
    // Проверяем, поддерживается ли извлечение текста
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Проверяем, поддерживается ли извлечение toc
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Получаем список таблиц
    IEnumerable<TocItem> toc = parser.GetToc();
    // Итерация по таблицам
    foreach (TocItem i in toc)
    {
        // Печатаем имя таблицы
        Console.WriteLine(i.Text);
        // Извлечь содержимое таблицы как текст
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Смотрите также

* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

Инициализирует новый экземпляр[`Parser`](../../parser) класс для извлечения данных из базы данных.

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| connection | DbConnection | Подключение к базе данных. |
| parserSettings | ParserSettings | Настройки парсера, которые используются для настройки извлечения данных. |

### Примечания

**Учить больше:**

* [Извлекать данные из баз данных](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [логирование](https://docs.groupdocs.com/display/parsernet/Logging)

### Примеры

В следующем примере показано, как извлечь данные из базы данных Sqlite:

```csharp
// Создаем объект DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Создаем экземпляр класса Parser для извлечения таблиц из базы данных
using (Parser parser = new Parser(connection))
{
    // Проверяем, поддерживается ли извлечение текста
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Проверяем, поддерживается ли извлечение toc
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Получаем список таблиц
    IEnumerable<TocItem> toc = parser.GetToc();
    // Итерация по таблицам
    foreach (TocItem i in toc)
    {
        // Печатаем имя таблицы
        Console.WriteLine(i.Text);
        // Извлечь содержимое таблицы как текст
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Смотрите также

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

Инициализирует новый экземпляр[`Parser`](../../parser) класс для извлечения данных с удаленного почтового сервера.

```csharp
public Parser(EmailConnection connection)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| connection | EmailConnection | Соединение с электронной почтой. |

### Примечания

**Учить больше:**

* [Извлечение электронных писем с удаленного сервера по протоколам POP, IMAP или Exchange Web Services.](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### Примеры

В следующем примере показано, как извлекать электронные письма из Exchange Server:

```csharp
// Создаем объект соединения для протокола Exchange Web Services 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx»,
    "email@server",
    "password");
 
// Создаем экземпляр класса Parser для извлечения писем с удаленного сервера
using (Parser parser = new Parser(connection))
{
    // Проверяем, поддерживается ли извлечение контейнера
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Извлечение сообщений электронной почты с сервера
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Перебираем вложения
    foreach (ContainerItem item in emails)
    {
        // Создаем экземпляр класса Parser для сообщения электронной почты
        using (Parser emailParser = item.OpenParser())
        {
            // Извлечь текст электронной почты
            using (TextReader reader = emailParser.GetText())
            {
                // Печатаем текст письма
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### Смотрите также

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

Инициализирует новый экземпляр[`Parser`](../../parser) класс для извлечения данных с удаленного почтового сервера.

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| connection | EmailConnection | Соединение с электронной почтой. |
| parserSettings | ParserSettings | Настройки парсера, которые используются для настройки извлечения данных. |

### Примечания

**Учить больше:**

* [Извлечение электронных писем с удаленного сервера по протоколам POP, IMAP или Exchange Web Services.](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [логирование](https://docs.groupdocs.com/display/parsernet/Logging)

### Примеры

В следующем примере показано, как извлекать электронные письма из Exchange Server:

```csharp
// Создаем объект соединения для протокола Exchange Web Services 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx»,
    "email@server",
    "password");
 
// Создаем экземпляр класса Parser для извлечения писем с удаленного сервера
using (Parser parser = new Parser(connection))
{
    // Проверяем, поддерживается ли извлечение контейнера
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Извлечение сообщений электронной почты с сервера
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Перебираем вложения
    foreach (ContainerItem item in emails)
    {
        // Создаем экземпляр класса Parser для сообщения электронной почты
        using (Parser emailParser = item.OpenParser())
        {
            // Извлечь текст электронной почты
            using (TextReader reader = emailParser.GetText())
            {
                // Печатаем текст письма
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### Смотрите также

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_7}

Инициализирует новый экземпляр[`Parser`](../../parser) класс.

```csharp
public Parser(string filePath)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | String | Путь к файлу. |

### Примечания

**Учить больше:**

* [Загрузить документ с локального диска](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Примеры

В следующем примере показано, как загрузить документ с локального диска:

```csharp
// Создаем экземпляр класса Parser с filePath
using (Parser parser = new Parser(filePath))
{
    // Извлечь текст в ридер
    using (TextReader reader = parser.GetText())
    {
        // Печатаем текст из документа
        // Если извлечение текста не поддерживается, читатель имеет значение null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Смотрите также

* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_8}

Инициализирует новый экземпляр[`Parser`](../../parser) класс с[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | String | Путь к файлу. |
| loadOptions | LoadOptions | Варианты открытия файла. |

### Примечания

**Учить больше:**

* [Загрузка определенных форматов файлов](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Загрузка защищенных паролем документов](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Загрузить документ с локального диска](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Примеры

Пароль документа передается классом LoadOptions:

```csharp
try
{
    // Создаем экземпляр класса Parser с паролем:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Проверяем, поддерживается ли извлечение текста
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Печатаем текст документа
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Печатаем сообщение, если пароль неверный или пустой
    Console.WriteLine("Invalid password");
}
```

### Смотрите также

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_9}

Инициализирует новый экземпляр[`Parser`](../../parser) класс с[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) и[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | String | Путь к файлу. |
| loadOptions | LoadOptions | Варианты открытия файла. |
| parserSettings | ParserSettings | Настройки парсера, которые используются для настройки извлечения данных. |

### Примечания

**Учить больше:**

* [Загрузка определенных форматов файлов](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Загрузка защищенных паролем документов](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [логирование](https://docs.groupdocs.com/display/parsernet/Logging)
* [Загрузить документ с локального диска](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Примеры

В следующем примере показано, как получить информацию через[`ILogger`](../../../groupdocs.parser.options/ilogger) интерфейс:

```csharp
// пытаться
{
    // Создаем экземпляр класса Logger
    Logger logger = new Logger();
    // Создаем экземпляр класса Parser с настройками парсера
    using (Parser parser = new Parser(filePath, null, new ParserSettings(logger)))
    {
        // Проверяем, поддерживается ли извлечение текста
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Печатаем текст документа
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // Игнорировать исключение
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // Распечатать сообщение об ошибке
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Распечатать сообщение о событии
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Печатаем предупреждающее сообщение
        Console.WriteLine("Warning: " + message);
    }
}
```

### Смотрите также

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

Инициализирует новый экземпляр[`Parser`](../../parser) класс.

```csharp
public Parser(Stream document)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| document | Stream | Исходный входной поток. |

### Примечания

**Учить больше:**

* [Загрузить документ из потока](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Примеры

В следующем примере показано, как загрузить документ из потока:

```csharp
// Создаем экземпляр класса Parser с потоком
using (Parser parser = new Parser(stream))
{
    // Извлечь текст в ридер
    using (TextReader reader = parser.GetText())
    {
        // Печатаем текст из документа
        // Если извлечение текста не поддерживается, читатель имеет значение null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Смотрите также

* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

Инициализирует новый экземпляр[`Parser`](../../parser) класс с[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| document | Stream | Исходный входной поток. |
| loadOptions | LoadOptions | Варианты открытия файла. |

### Примечания

**Учить больше:**

* [Загрузка определенных форматов файлов](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Загрузка защищенных паролем документов](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Загрузить документ из потока](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Примеры

В некоторых случаях необходимо определить[`FileFormat`](../../../groupdocs.parser.options/fileformat). Как для частных случаев (базы данных, почтовый сервер), так и для определения типов файлов по содержимому:

Пароль документа передается[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) учебный класс:

```csharp
// Создаем экземпляр класса Parser для документа уценки
using (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup)))
{
    // Проверяем, поддерживается ли извлечение текста
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    using (TextReader reader = parser.GetText())
    {
        // Печатаем текст документа
        // Обнаружена уценка; печатается текст без специальных символов
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

```csharp
try
{
    // Создаем экземпляр класса Parser с паролем:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Проверяем, поддерживается ли извлечение текста
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Печатаем текст документа
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Печатаем сообщение, если пароль неверный или пустой
    Console.WriteLine("Invalid password");
}
```

### Смотрите также

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

Инициализирует новый экземпляр[`Parser`](../../parser) класс с[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) и[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| document | Stream | Исходный входной поток. |
| loadOptions | LoadOptions | Варианты открытия файла. |
| parserSettings | ParserSettings | Настройки парсера, которые используются для настройки извлечения данных. |

### Примечания

**Учить больше:**

* [Загрузка определенных форматов файлов](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Загрузка защищенных паролем документов](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Загрузить документ из потока](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [логирование](https://docs.groupdocs.com/display/parsernet/Logging)

### Примеры

В следующем примере показано, как получить информацию через[`ILogger`](../../../groupdocs.parser.options/ilogger) интерфейс:

```csharp
// пытаться
{
    // Создаем экземпляр класса Logger
    Logger logger = new Logger();
    // Создаем экземпляр класса Parser с настройками парсера
    using (Parser parser = new Parser(stream, null, new ParserSettings(logger)))
    {
        // Проверяем, поддерживается ли извлечение текста
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Печатаем текст документа
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // Игнорировать исключение
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // Распечатать сообщение об ошибке
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Распечатать сообщение о событии
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Печатаем предупреждающее сообщение
        Console.WriteLine("Warning: " + message);
    }
}
```

### Смотрите также

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

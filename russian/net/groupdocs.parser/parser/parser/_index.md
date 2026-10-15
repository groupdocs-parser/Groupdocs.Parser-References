---
title: "Parser"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Инициализирует новый экземпляр класса Parsergroupdocs.parser/parser для извлечения данных из URI."
type: docs
weight: 10
url: /ru/net/groupdocs.parser/parser/parser/
---

## Parser(Uri) {#constructor_12}

Инициализирует новый экземпляр класса [`Parser`](../../parser) для извлечения данных из URI.

```csharp
public Parser(Uri uri)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| uri | Uri | URI, к которому отправляется запрос. |

### См. также

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions) {#constructor_13}

Инициализирует новый экземпляр класса [`Parser`](../../parser) для извлечения данных из URI с *loadOptions*.

```csharp
public Parser(Uri uri, LoadOptions loadOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| uri | Uri | URI, к которому отправляется запрос. |
| loadOptions | LoadOptions | Параметры открытия файла. |

### См. также

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, ParserSettings) {#constructor_15}

Инициализирует новый экземпляр класса [`Parser`](../../parser) для извлечения данных из URI с *parserSettings*.

```csharp
public Parser(Uri uri, ParserSettings parserSettings)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| uri | Uri | URI, к которому отправляется запрос. |
| parserSettings | ParserSettings | Настройки парсера, используемые для настройки извлечения данных. |

### См. также

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions, ParserSettings) {#constructor_14}

Инициализирует новый экземпляр класса [`Parser`](../../parser) для извлечения данных из URI с *loadOptions* и *parserSettings*.

```csharp
public Parser(Uri uri, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| uri | Uri | URI, к которому отправляется запрос. |
| loadOptions | LoadOptions | Параметры открытия файла. |
| parserSettings | ParserSettings | Настройки парсера, используемые для настройки извлечения данных. |

### См. также

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection) {#constructor_2}

Инициализирует новый экземпляр класса [`Parser`](../../parser) для извлечения данных из базы данных.

```csharp
public Parser(DbConnection connection)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| соединение | DbConnection | Подключение к базе данных. |

### Примечания

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### Примеры

В следующем примере показано, как извлекать данные из базы данных Sqlite:

```csharp
// Создать объект DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Создать экземпляр класса Parser для извлечения таблиц из базы данных
using (Parser parser = new Parser(connection))
{
    // Проверьте, поддерживается ли извлечение текста
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Проверьте, поддерживается ли извлечение оглавления
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Получить список таблиц
    IEnumerable<TocItem> toc = parser.GetToc();
    // Перебрать таблицы
    foreach (TocItem i in toc)
    {
        // Вывести имя таблицы
        Console.WriteLine(i.Text);
        // Извлечь содержимое таблицы в виде текста
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### См. также

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

Инициализирует новый экземпляр класса [`Parser`](../../parser) для извлечения данных из базы данных.

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| соединение | DbConnection | Подключение к базе данных. |
| parserSettings | ParserSettings | Настройки парсера, используемые для настройки извлечения данных. |

### Примечания

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Примеры

В следующем примере показано, как извлекать данные из базы данных Sqlite:

```csharp
// Создать объект DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Создать экземпляр класса Parser для извлечения таблиц из базы данных
using (Parser parser = new Parser(connection))
{
    // Проверьте, поддерживается ли извлечение текста
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Проверьте, поддерживается ли извлечение оглавления
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Получить список таблиц
    IEnumerable<TocItem> toc = parser.GetToc();
    // Перебрать таблицы
    foreach (TocItem i in toc)
    {
        // Вывести имя таблицы
        Console.WriteLine(i.Text);
        // Извлечь содержимое таблицы в виде текста
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### См. также

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

Инициализирует новый экземпляр класса [`Parser`](../../parser) для извлечения данных с удалённого почтового сервера.

```csharp
public Parser(EmailConnection connection)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| соединение | EmailConnection | Подключение к электронной почте. |

### Примечания

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### Примеры

В следующем примере показано, как извлекать электронные письма с Exchange Server:

```csharp
// Создать объект соединения для протокола Exchange Web Services
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Создать экземпляр класса Parser для извлечения электронных писем с удалённого сервера
using (Parser parser = new Parser(connection))
{
    // Проверьте, поддерживается ли извлечение контейнера
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Извлечь сообщения электронной почты с сервера
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Переберите вложения
    foreach (ContainerItem item in emails)
    {
        // Создайте экземпляр класса Parser для сообщения электронной почты
        using (Parser emailParser = item.OpenParser())
        {
            // Извлеките текст письма
            using (TextReader reader = emailParser.GetText())
            {
                // Выведите текст письма
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### См. также

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

Инициализирует новый экземпляр класса [`Parser`](../../parser) для извлечения данных с удалённого почтового сервера.

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| соединение | EmailConnection | Подключение к электронной почте. |
| parserSettings | ParserSettings | Настройки парсера, используемые для настройки извлечения данных. |

### Примечания

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Примеры

В следующем примере показано, как извлекать электронные письма с Exchange Server:

```csharp
// Создать объект соединения для протокола Exchange Web Services
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Создать экземпляр класса Parser для извлечения электронных писем с удалённого сервера
using (Parser parser = new Parser(connection))
{
    // Проверьте, поддерживается ли извлечение контейнера
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Извлечь сообщения электронной почты с сервера
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Переберите вложения
    foreach (ContainerItem item in emails)
    {
        // Создайте экземпляр класса Parser для сообщения электронной почты
        using (Parser emailParser = item.OpenParser())
        {
            // Извлеките текст письма
            using (TextReader reader = emailParser.GetText())
            {
                // Выведите текст письма
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### См. также

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_8}

Инициализирует новый экземпляр класса [`Parser`](../../parser).

```csharp
public Parser(string filePath)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | Строка | Путь к файлу. |

### Примечания

**Learn more:**

* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Примеры

В следующем примере показано, как загрузить документ с локального диска:

```csharp
// Создайте экземпляр класса Parser с указанием пути к файлу
using (Parser parser = new Parser(filePath))
{
    // Извлечь текст в reader
    using (TextReader reader = parser.GetText())
    {
        // Вывести текст из документа
        // Если извлечение текста не поддерживается, reader будет null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### См. также

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_9}

Инициализирует новый экземпляр класса [`Parser`](../../parser) с помощью [`LoadOptions`](../../../groupdocs.parser.options/loadoptions).

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | Строка | Путь к файлу. |
| loadOptions | LoadOptions | Параметры открытия файла. |

### Примечания

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Примеры

Пароль документа передаётся классом LoadOptions:

```csharp
try
{
    // Создайте экземпляр класса Parser с паролем:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Проверьте, поддерживается ли извлечение текста
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Выведите текст документа
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Выведите сообщение, если пароль неверен или пуст
    Console.WriteLine("Invalid password");
}
```

### См. также

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, ParserSettings) {#constructor_11}

Инициализирует новый экземпляр класса [`Parser`](../../parser) с помощью [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(string filePath, ParserSettings parserSettings)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | Строка | Путь к файлу. |
| parserSettings | ParserSettings | Настройки парсера, используемые для настройки извлечения данных. |

### См. также

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_10}

Инициализирует новый экземпляр класса [`Parser`](../../parser) с помощью [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) и [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | Строка | Путь к файлу. |
| loadOptions | LoadOptions | Параметры открытия файла. |
| parserSettings | ParserSettings | Настройки парсера, используемые для настройки извлечения данных. |

### Примечания

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Примеры

В следующем примере показано, как получить информацию через интерфейс [`ILogger`](../../../groupdocs.parser.options/ilogger):

```csharp
// try
{
    // Создайте экземпляр класса Logger
    Logger logger = new Logger();
    // Создайте экземпляр класса Parser с настройками парсера
    using (Parser parser = new Parser(filePath, null, new ParserSettings(logger)))
    {
        // Проверьте, поддерживается ли извлечение текста
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Выведите текст документа
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // Ignore the exception
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // Выведите сообщение об ошибке
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Выведите сообщение о событии
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Выведите предупреждающее сообщение
        Console.WriteLine("Warning: " + message);
    }
}
```

### См. также

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

Инициализирует новый экземпляр класса [`Parser`](../../parser).

```csharp
public Parser(Stream document)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| документ | Stream | Исходный входной поток. |

### Примечания

**Learn more:**

* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Примеры

В следующем примере показано, как загрузить документ из потока:

```csharp
// Создайте экземпляр класса Parser с потоком
using (Parser parser = new Parser(stream))
{
    // Извлечь текст в reader
    using (TextReader reader = parser.GetText())
    {
        // Вывести текст из документа
        // Если извлечение текста не поддерживается, reader будет null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### См. также

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

Инициализирует новый экземпляр класса [`Parser`](../../parser) с помощью [`LoadOptions`](../../../groupdocs.parser.options/loadoptions).

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| документ | Stream | Исходный входной поток. |
| loadOptions | LoadOptions | Параметры открытия файла. |

### Примечания

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Примеры

В некоторых случаях необходимо определить [`FileFormat`](../../../groupdocs.parser.options/fileformat). Как для специальных случаев (базы данных, сервер электронной почты), так и для определения типов файлов по содержимому:

```csharp
// Создайте экземпляр класса Parser для markdown‑документа
using (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup)))
{
    // Проверьте, поддерживается ли извлечение текста
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    using (TextReader reader = parser.GetText())
    {
        // Выведите текст документа
        // Обнаружен markdown; текст без специальных символов выводится
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

Пароль документа передаётся классом [`LoadOptions`](../../../groupdocs.parser.options/loadoptions):

```csharp
try
{
    // Создайте экземпляр класса Parser с паролем:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Проверьте, поддерживается ли извлечение текста
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Выведите текст документа
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Выведите сообщение, если пароль неверен или пуст
    Console.WriteLine("Invalid password");
}
```

### См. также

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, ParserSettings) {#constructor_7}

Инициализирует новый экземпляр класса [`Parser`](../../parser) с помощью [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(Stream document, ParserSettings parserSettings)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| документ | Stream | Исходный входной поток. |
| parserSettings | ParserSettings | Настройки парсера, используемые для настройки извлечения данных. |

### См. также

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

Инициализирует новый экземпляр класса [`Parser`](../../parser) с помощью [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) и [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| документ | Stream | Исходный входной поток. |
| loadOptions | LoadOptions | Параметры открытия файла. |
| parserSettings | ParserSettings | Настройки парсера, используемые для настройки извлечения данных. |

### Примечания

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Примеры

В следующем примере показано, как получить информацию через интерфейс [`ILogger`](../../../groupdocs.parser.options/ilogger):

```csharp
// try
{
    // Создайте экземпляр класса Logger
    Logger logger = new Logger();
    // Создайте экземпляр класса Parser с настройками парсера
    using (Parser parser = new Parser(stream, null, new ParserSettings(logger)))
    {
        // Проверьте, поддерживается ли извлечение текста
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Выведите текст документа
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // Ignore the exception
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // Выведите сообщение об ошибке
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Выведите сообщение о событии
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Выведите предупреждающее сообщение
        Console.WriteLine("Warning: " + message);
    }
}
```

### См. также

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->

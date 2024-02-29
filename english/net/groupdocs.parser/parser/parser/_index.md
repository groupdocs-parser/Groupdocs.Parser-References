---
title: Parser
second_title: GroupDocs.Parser for .NET API Reference
description: Initializes a new instance of the Parsergroupdocs.parser/parser class to extract data from an URI.
type: docs
weight: 10
url: /net/groupdocs.parser/parser/parser/
---
## Parser(Uri) {#constructor_12}

Initializes a new instance of the [`Parser`](../../parser) class to extract data from an URI.

```csharp
public Parser(Uri uri)
```

| Parameter | Type | Description |
| --- | --- | --- |
| uri | Uri | The Uri the request is sent to. |

### See Also

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions) {#constructor_13}

Initializes a new instance of the [`Parser`](../../parser) class to extract data from an URI with *loadOptions*.

```csharp
public Parser(Uri uri, LoadOptions loadOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| uri | Uri | The Uri the request is sent to. |
| loadOptions | LoadOptions | The options to open the file. |

### See Also

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, ParserSettings) {#constructor_15}

Initializes a new instance of the [`Parser`](../../parser) class to extract data from an URI with *parserSettings*.

```csharp
public Parser(Uri uri, ParserSettings parserSettings)
```

| Parameter | Type | Description |
| --- | --- | --- |
| uri | Uri | The Uri the request is sent to. |
| parserSettings | ParserSettings | The parser settings which are used to customize data extraction. |

### See Also

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions, ParserSettings) {#constructor_14}

Initializes a new instance of the [`Parser`](../../parser) class to extract data from an URI with *loadOptions* and *parserSettings*.

```csharp
public Parser(Uri uri, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | Description |
| --- | --- | --- |
| uri | Uri | The Uri the request is sent to. |
| loadOptions | LoadOptions | The options to open the file. |
| parserSettings | ParserSettings | The parser settings which are used to customize data extraction. |

### See Also

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection) {#constructor_2}

Initializes a new instance of the [`Parser`](../../parser) class to extract data from a database.

```csharp
public Parser(DbConnection connection)
```

| Parameter | Type | Description |
| --- | --- | --- |
| connection | DbConnection | The database connection. |

### Remarks

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### Examples

The following example shows how to extract data from Sqlite database:

```csharp
// Create DbConnection object
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Create an instance of Parser class to extract tables from the database
using (Parser parser = new Parser(connection))
{
    // Check if text extraction is supported
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Check if toc extraction is supported
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Get a list of tables
    IEnumerable<TocItem> toc = parser.GetToc();
    // Iterate over tables
    foreach (TocItem i in toc)
    {
        // Print the table name
        Console.WriteLine(i.Text);
        // Extract a table content as a text
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### See Also

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

Initializes a new instance of the [`Parser`](../../parser) class to extract data from a database.

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| Parameter | Type | Description |
| --- | --- | --- |
| connection | DbConnection | The database connection. |
| parserSettings | ParserSettings | The parser settings which are used to customize data extraction. |

### Remarks

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Examples

The following example shows how to extract data from Sqlite database:

```csharp
// Create DbConnection object
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Create an instance of Parser class to extract tables from the database
using (Parser parser = new Parser(connection))
{
    // Check if text extraction is supported
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Check if toc extraction is supported
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Get a list of tables
    IEnumerable<TocItem> toc = parser.GetToc();
    // Iterate over tables
    foreach (TocItem i in toc)
    {
        // Print the table name
        Console.WriteLine(i.Text);
        // Extract a table content as a text
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### See Also

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

Initializes a new instance of the [`Parser`](../../parser) class to extract data from a remote email server.

```csharp
public Parser(EmailConnection connection)
```

| Parameter | Type | Description |
| --- | --- | --- |
| connection | EmailConnection | The email connection. |

### Remarks

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### Examples

The following example shows how to extract emails from Exchange Server:

```csharp
// Create the connection object for Exchange Web Services protocol 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Create an instance of Parser class to extract emails from the remote server
using (Parser parser = new Parser(connection))
{
    // Check if container extraction is supported
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Extract email messages from the server
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Iterate over attachments
    foreach (ContainerItem item in emails)
    {
        // Create an instance of Parser class for email message
        using (Parser emailParser = item.OpenParser())
        {
            // Extract the email text
            using (TextReader reader = emailParser.GetText())
            {
                // Print the email text
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### See Also

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

Initializes a new instance of the [`Parser`](../../parser) class to extract data from a remote email server.

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| Parameter | Type | Description |
| --- | --- | --- |
| connection | EmailConnection | The email connection. |
| parserSettings | ParserSettings | The parser settings which are used to customize data extraction. |

### Remarks

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Examples

The following example shows how to extract emails from Exchange Server:

```csharp
// Create the connection object for Exchange Web Services protocol 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Create an instance of Parser class to extract emails from the remote server
using (Parser parser = new Parser(connection))
{
    // Check if container extraction is supported
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Extract email messages from the server
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Iterate over attachments
    foreach (ContainerItem item in emails)
    {
        // Create an instance of Parser class for email message
        using (Parser emailParser = item.OpenParser())
        {
            // Extract the email text
            using (TextReader reader = emailParser.GetText())
            {
                // Print the email text
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### See Also

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_8}

Initializes a new instance of the [`Parser`](../../parser) class.

```csharp
public Parser(string filePath)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filePath | String | The path to the file. |

### Remarks

**Learn more:**

* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Examples

The following example shows how to load the document from the local disk:

```csharp
// Create an instance of Parser class with the filePath
using (Parser parser = new Parser(filePath))
{
    // Extract a text into the reader
    using (TextReader reader = parser.GetText())
    {
        // Print a text from the document
        // If text extraction isn't supported, a reader is null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### See Also

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_9}

Initializes a new instance of the [`Parser`](../../parser) class with [`LoadOptions`](../../../groupdocs.parser.options/loadoptions).

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filePath | String | The path to the file. |
| loadOptions | LoadOptions | The options to open the file. |

### Remarks

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Examples

The document password is passed by LoadOptions class:

```csharp
try
{
    // Create an instance of Parser class with the password:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Check if text extraction is supported
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Print the document text
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Print the message if the password is incorrect or empty
    Console.WriteLine("Invalid password");
}
```

### See Also

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, ParserSettings) {#constructor_11}

Initializes a new instance of the [`Parser`](../../parser) class with [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(string filePath, ParserSettings parserSettings)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filePath | String | The path to the file. |
| parserSettings | ParserSettings | The parser settings which are used to customize data extraction. |

### See Also

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_10}

Initializes a new instance of the [`Parser`](../../parser) class with [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) and [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filePath | String | The path to the file. |
| loadOptions | LoadOptions | The options to open the file. |
| parserSettings | ParserSettings | The parser settings which are used to customize data extraction. |

### Remarks

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Examples

The following example shows how to receive the information via [`ILogger`](../../../groupdocs.parser.options/ilogger) interface:

```csharp
// try
{
    // Create an instance of Logger class
    Logger logger = new Logger();
    // Create an instance of Parser class with the parser settings
    using (Parser parser = new Parser(filePath, null, new ParserSettings(logger)))
    {
        // Check if text extraction is supported
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Print the document text
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
        // Print error message
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Print event message
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Print warning message
        Console.WriteLine("Warning: " + message);
    }
}
```

### See Also

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

Initializes a new instance of the [`Parser`](../../parser) class.

```csharp
public Parser(Stream document)
```

| Parameter | Type | Description |
| --- | --- | --- |
| document | Stream | The source input stream. |

### Remarks

**Learn more:**

* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Examples

The following example shows how to load the document from the stream:

```csharp
// Create an instance of Parser class with the stream
using (Parser parser = new Parser(stream))
{
    // Extract a text into the reader
    using (TextReader reader = parser.GetText())
    {
        // Print a text from the document
        // If text extraction isn't supported, a reader is null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### See Also

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

Initializes a new instance of the [`Parser`](../../parser) class with [`LoadOptions`](../../../groupdocs.parser.options/loadoptions).

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| document | Stream | The source input stream. |
| loadOptions | LoadOptions | The options to open the file. |

### Remarks

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Examples

In some cases it's necessary to define [`FileFormat`](../../../groupdocs.parser.options/fileformat). Both for special cases (databases, email server) and for detecting file types by the content:

```csharp
// Create an instance of Parser class for markdown document
using (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup)))
{
    // Check if text extraction is supported
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    using (TextReader reader = parser.GetText())
    {
        // Print the document text
        // Markdown is detected; text without special symbols is printed
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

The document password is passed by [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) class:

```csharp
try
{
    // Create an instance of Parser class with the password:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Check if text extraction is supported
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Print the document text
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Print the message if the password is incorrect or empty
    Console.WriteLine("Invalid password");
}
```

### See Also

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, ParserSettings) {#constructor_7}

Initializes a new instance of the [`Parser`](../../parser) class with [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(Stream document, ParserSettings parserSettings)
```

| Parameter | Type | Description |
| --- | --- | --- |
| document | Stream | The source input stream. |
| parserSettings | ParserSettings | The parser settings which are used to customize data extraction. |

### See Also

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

Initializes a new instance of the [`Parser`](../../parser) class with [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) and [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | Description |
| --- | --- | --- |
| document | Stream | The source input stream. |
| loadOptions | LoadOptions | The options to open the file. |
| parserSettings | ParserSettings | The parser settings which are used to customize data extraction. |

### Remarks

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Examples

The following example shows how to receive the information via [`ILogger`](../../../groupdocs.parser.options/ilogger) interface:

```csharp
// try
{
    // Create an instance of Logger class
    Logger logger = new Logger();
    // Create an instance of Parser class with the parser settings
    using (Parser parser = new Parser(stream, null, new ParserSettings(logger)))
    {
        // Check if text extraction is supported
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Print the document text
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
        // Print error message
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Print event message
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Print warning message
        Console.WriteLine("Warning: " + message);
    }
}
```

### See Also

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.parser.dll -->

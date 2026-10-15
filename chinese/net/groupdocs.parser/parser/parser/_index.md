---
title: "解析器"
second_title: "GroupDocs.Parser for .NET API 参考"
description: "初始化 Parsergroupdocs.parser/parser 类的新实例以从 URI 提取数据。"
type: docs
weight: 10
url: /zh/net/groupdocs.parser/parser/parser/
---

## Parser(Uri) {#constructor_12}

初始化 [`Parser`](../../parser) 类的新实例以从 URI 提取数据。

```csharp
public Parser(Uri uri)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| uri | Uri | 请求发送到的 Uri。 |

### 另请参见

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions) {#constructor_13}

初始化一个新的 [`Parser`](../../parser) 类实例，以使用 *loadOptions* 从 URI 提取数据。

```csharp
public Parser(Uri uri, LoadOptions loadOptions)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| uri | Uri | 请求发送到的 Uri。 |
| loadOptions | LoadOptions | 打开文件的选项。 |

### 另请参见

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, ParserSettings) {#constructor_15}

初始化一个新的 [`Parser`](../../parser) 类实例，以使用 *parserSettings* 从 URI 提取数据。

```csharp
public Parser(Uri uri, ParserSettings parserSettings)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| uri | Uri | 请求发送到的 Uri。 |
| parserSettings | ParserSettings | 用于自定义数据提取的解析器设置。 |

### 另请参见

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions, ParserSettings) {#constructor_14}

初始化一个新的 [`Parser`](../../parser) 类实例，以使用 *loadOptions* 和 *parserSettings* 从 URI 提取数据。

```csharp
public Parser(Uri uri, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| uri | Uri | 请求发送到的 Uri。 |
| loadOptions | LoadOptions | 打开文件的选项。 |
| parserSettings | ParserSettings | 用于自定义数据提取的解析器设置。 |

### 另请参见

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection) {#constructor_2}

初始化一个新的 [`Parser`](../../parser) 类实例，以从数据库提取数据。

```csharp
public Parser(DbConnection connection)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 连接 | DbConnection | 数据库连接。 |

### 备注

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### 示例

下面的示例展示了如何从 Sqlite 数据库提取数据：

```csharp
// 创建 DbConnection 对象
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// 创建 Parser 类的实例以从数据库提取表
using (Parser parser = new Parser(connection))
{
    // 检查是否支持文本提取
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // 检查是否支持目录提取
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // 获取表列表
    IEnumerable<TocItem> toc = parser.GetToc();
    // 遍历表
    foreach (TocItem i in toc)
    {
        // 打印表名
        Console.WriteLine(i.Text);
        // 将表内容提取为文本
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### 另请参见

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

初始化一个新的 [`Parser`](../../parser) 类实例，以从数据库提取数据。

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 连接 | DbConnection | 数据库连接。 |
| parserSettings | ParserSettings | 用于自定义数据提取的解析器设置。 |

### 备注

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### 示例

下面的示例展示了如何从 Sqlite 数据库提取数据：

```csharp
// 创建 DbConnection 对象
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// 创建 Parser 类的实例以从数据库提取表
using (Parser parser = new Parser(connection))
{
    // 检查是否支持文本提取
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // 检查是否支持目录提取
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // 获取表列表
    IEnumerable<TocItem> toc = parser.GetToc();
    // 遍历表
    foreach (TocItem i in toc)
    {
        // 打印表名
        Console.WriteLine(i.Text);
        // 将表内容提取为文本
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### 另请参见

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

初始化一个新的 [`Parser`](../../parser) 类实例，以从远程电子邮件服务器提取数据。

```csharp
public Parser(EmailConnection connection)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 连接 | EmailConnection | 电子邮件连接。 |

### 备注

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### 示例

下面的示例展示了如何从 Exchange Server 提取电子邮件：

```csharp
// 为 Exchange Web Services 协议创建连接对象 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// 创建 Parser 类的实例以从远程服务器提取电子邮件
using (Parser parser = new Parser(connection))
{
    // 检查是否支持容器提取
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// 从服务器提取电子邮件消息
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // 遍历附件
    foreach (ContainerItem item in emails)
    {
        // 为电子邮件消息创建 Parser 类的实例
        using (Parser emailParser = item.OpenParser())
        {
            // 提取电子邮件文本
            using (TextReader reader = emailParser.GetText())
            {
                // 打印电子邮件文本
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### 另请参见

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

初始化一个新的 [`Parser`](../../parser) 类实例，以从远程电子邮件服务器提取数据。

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 连接 | EmailConnection | 电子邮件连接。 |
| parserSettings | ParserSettings | 用于自定义数据提取的解析器设置。 |

### 备注

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### 示例

下面的示例展示了如何从 Exchange Server 提取电子邮件：

```csharp
// 为 Exchange Web Services 协议创建连接对象 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// 创建 Parser 类的实例以从远程服务器提取电子邮件
using (Parser parser = new Parser(connection))
{
    // 检查是否支持容器提取
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// 从服务器提取电子邮件消息
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // 遍历附件
    foreach (ContainerItem item in emails)
    {
        // 为电子邮件消息创建 Parser 类的实例
        using (Parser emailParser = item.OpenParser())
        {
            // 提取电子邮件文本
            using (TextReader reader = emailParser.GetText())
            {
                // 打印电子邮件文本
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### 另请参见

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_8}

初始化一个新的 [`Parser`](../../parser) 类实例。

```csharp
public Parser(string filePath)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| filePath | 字符串 | 文件的路径。 |

### 备注

**Learn more:**

* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### 示例

下面的示例展示了如何从本地磁盘加载文档：

```csharp
// 使用 filePath 创建 Parser 类的实例
using (Parser parser = new Parser(filePath))
{
    // 将文本提取到读取器中
    using (TextReader reader = parser.GetText())
    {
        // 打印文档中的文本
        // 如果不支持文本提取，reader 为 null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### 另请参见

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_9}

使用 [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) 初始化 [`Parser`](../../parser) 类的新实例。

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| filePath | 字符串 | 文件的路径。 |
| loadOptions | LoadOptions | 打开文件的选项。 |

### 备注

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### 示例

文档密码通过 LoadOptions 类传递：

```csharp
try
{
    // 使用密码创建 Parser 类的实例：
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // 检查是否支持文本提取
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // 打印文档文本
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // 如果密码不正确或为空，打印消息
    Console.WriteLine("Invalid password");
}
```

### 另请参见

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, ParserSettings) {#constructor_11}

使用 [`ParserSettings`](../../../groupdocs.parser.options/parsersettings) 初始化 [`Parser`](../../parser) 类的新实例。

```csharp
public Parser(string filePath, ParserSettings parserSettings)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| filePath | 字符串 | 文件的路径。 |
| parserSettings | ParserSettings | 用于自定义数据提取的解析器设置。 |

### 另请参见

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_10}

使用 [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) 和 [`ParserSettings`](../../../groupdocs.parser.options/parsersettings) 初始化 [`Parser`](../../parser) 类的新实例。

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| filePath | 字符串 | 文件的路径。 |
| loadOptions | LoadOptions | 打开文件的选项。 |
| parserSettings | ParserSettings | 用于自定义数据提取的解析器设置。 |

### 备注

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### 示例

下面的示例展示了如何通过 [`ILogger`](../../../groupdocs.parser.options/ilogger) 接口获取信息：

```csharp
// try
{
    // 创建 Logger 类的实例
    Logger logger = new Logger();
    // 使用解析器设置创建 Parser 类的实例
    using (Parser parser = new Parser(filePath, null, new ParserSettings(logger)))
    {
        // 检查是否支持文本提取
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // 打印文档文本
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
        // 打印错误信息
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // 打印事件信息
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // 打印警告信息
        Console.WriteLine("Warning: " + message);
    }
}
```

### 另请参见

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

初始化一个新的 [`Parser`](../../parser) 类实例。

```csharp
public Parser(Stream document)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 文档 | Stream | 源输入流。 |

### 备注

**Learn more:**

* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### 示例

下面的示例展示了如何从流加载文档：

```csharp
// 使用流创建 Parser 类的实例
using (Parser parser = new Parser(stream))
{
    // 将文本提取到读取器中
    using (TextReader reader = parser.GetText())
    {
        // 打印文档中的文本
        // 如果不支持文本提取，reader 为 null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### 另请参见

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

使用 [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) 初始化 [`Parser`](../../parser) 类的新实例。

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 文档 | Stream | 源输入流。 |
| loadOptions | LoadOptions | 打开文件的选项。 |

### 备注

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### 示例

在某些情况下，需要定义 [`FileFormat`](../../../groupdocs.parser.options/fileformat)。这既适用于特殊情况（数据库、邮件服务器），也适用于通过内容检测文件类型：

```csharp
// 为 Markdown 文档创建 Parser 类的实例
using (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup)))
{
    // 检查是否支持文本提取
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    using (TextReader reader = parser.GetText())
    {
        // 打印文档文本
        // 检测到 Markdown；打印没有特殊符号的文本
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

文档密码通过 [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) 类传递：

```csharp
try
{
    // 使用密码创建 Parser 类的实例：
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // 检查是否支持文本提取
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // 打印文档文本
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // 如果密码不正确或为空，打印消息
    Console.WriteLine("Invalid password");
}
```

### 另请参见

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, ParserSettings) {#constructor_7}

使用 [`ParserSettings`](../../../groupdocs.parser.options/parsersettings) 初始化 [`Parser`](../../parser) 类的新实例。

```csharp
public Parser(Stream document, ParserSettings parserSettings)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 文档 | Stream | 源输入流。 |
| parserSettings | ParserSettings | 用于自定义数据提取的解析器设置。 |

### 另请参见

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

使用 [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) 和 [`ParserSettings`](../../../groupdocs.parser.options/parsersettings) 初始化 [`Parser`](../../parser) 类的新实例。

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 文档 | Stream | 源输入流。 |
| loadOptions | LoadOptions | 打开文件的选项。 |
| parserSettings | ParserSettings | 用于自定义数据提取的解析器设置。 |

### 备注

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### 示例

下面的示例展示了如何通过 [`ILogger`](../../../groupdocs.parser.options/ilogger) 接口获取信息：

```csharp
// try
{
    // 创建 Logger 类的实例
    Logger logger = new Logger();
    // 使用解析器设置创建 Parser 类的实例
    using (Parser parser = new Parser(stream, null, new ParserSettings(logger)))
    {
        // 检查是否支持文本提取
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // 打印文档文本
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
        // 打印错误信息
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // 打印事件信息
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // 打印警告信息
        Console.WriteLine("Warning: " + message);
    }
}
```

### 另请参见

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

---
title: Parser
second_title: GroupDocs.Parser for .NET API 参考
description: 初始化一个新的实例Parsergroupdocs.parser/parser从数据库中提取数据的类
type: docs
weight: 10
url: /zh/net/groupdocs.parser/parser/parser/
---
## Parser(DbConnection) {#constructor_2}

初始化一个新的实例[`Parser`](../../parser)从数据库中提取数据的类。

```csharp
public Parser(DbConnection connection)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| connection | DbConnection | 数据库连接。 |

### 评论

**了解更多：**

* [从数据库中提取数据](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### 例子

下面的例子展示了如何从 Sqlite 数据库中提取数据：

```csharp
// 创建 DbConnection 对象
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// 创建 Parser 类的实例以从数据库中提取表
using (Parser parser = new Parser(connection))
{
    // 检查是否支持文本提取
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // 检查是否支持 toc 提取
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // 获取表格列表
    IEnumerable<TocItem> toc = parser.GetToc();
    // 遍历表
    foreach (TocItem i in toc)
    {
        //打印表名
        Console.WriteLine(i.Text);
        // 将表格内容提取为文本
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### 也可以看看

* class [Parser](../../parser)
* 命名空间 [GroupDocs.Parser](../../parser)
* 部件 [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

初始化一个新的实例[`Parser`](../../parser)从数据库中提取数据的类。

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| connection | DbConnection | 数据库连接。 |
| parserSettings | ParserSettings | 用于自定义数据提取的解析器设置。 |

### 评论

**了解更多：**

* [从数据库中提取数据](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [记录](https://docs.groupdocs.com/display/parsernet/Logging)

### 例子

下面的例子展示了如何从 Sqlite 数据库中提取数据：

```csharp
// 创建 DbConnection 对象
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// 创建 Parser 类的实例以从数据库中提取表
using (Parser parser = new Parser(connection))
{
    // 检查是否支持文本提取
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // 检查是否支持 toc 提取
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // 获取表格列表
    IEnumerable<TocItem> toc = parser.GetToc();
    // 遍历表
    foreach (TocItem i in toc)
    {
        //打印表名
        Console.WriteLine(i.Text);
        // 将表格内容提取为文本
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### 也可以看看

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* 命名空间 [GroupDocs.Parser](../../parser)
* 部件 [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

初始化一个新的实例[`Parser`](../../parser)从远程电子邮件服务器中提取数据的类。

```csharp
public Parser(EmailConnection connection)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| connection | EmailConnection | 电子邮件连接。 |

### 评论

**了解更多：**

* [通过 POP、IMAP 或 Exchange Web 服务协议从远程服务器提取电子邮件](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### 例子

以下示例显示如何从 Exchange Server 中提取电子邮件：

```csharp
// 为 Exchange Web 服务协议创建连接对象 
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

// 从服务器中提取电子邮件信息
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // 遍历附件
    foreach (ContainerItem item in emails)
    {
        // 为电子邮件创建 Parser 类的实例
        using (Parser emailParser = item.OpenParser())
        {
            // 提取邮件文本
            using (TextReader reader = emailParser.GetText())
            {
                // 打印邮件文本
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### 也可以看看

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* 命名空间 [GroupDocs.Parser](../../parser)
* 部件 [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

初始化一个新的实例[`Parser`](../../parser)从远程电子邮件服务器中提取数据的类。

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| connection | EmailConnection | 电子邮件连接。 |
| parserSettings | ParserSettings | 用于自定义数据提取的解析器设置。 |

### 评论

**了解更多：**

* [通过 POP、IMAP 或 Exchange Web 服务协议从远程服务器提取电子邮件](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [记录](https://docs.groupdocs.com/display/parsernet/Logging)

### 例子

以下示例显示如何从 Exchange Server 中提取电子邮件：

```csharp
// 为 Exchange Web 服务协议创建连接对象 
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

// 从服务器中提取电子邮件信息
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // 遍历附件
    foreach (ContainerItem item in emails)
    {
        // 为电子邮件创建 Parser 类的实例
        using (Parser emailParser = item.OpenParser())
        {
            // 提取邮件文本
            using (TextReader reader = emailParser.GetText())
            {
                // 打印邮件文本
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### 也可以看看

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* 命名空间 [GroupDocs.Parser](../../parser)
* 部件 [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_8}

初始化一个新的实例[`Parser`](../../parser)类.

```csharp
public Parser(string filePath)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| filePath | String | 文件的路径。 |

### 评论

**了解更多：**

* [从本地磁盘加载文档](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### 例子

以下示例显示如何从本地磁盘加载文档：

```csharp
// 使用文件路径创建 Parser 类的实例
using (Parser parser = new Parser(filePath))
{
    // 将文本提取到阅读器中
    using (TextReader reader = parser.GetText())
    {
        // 打印文档中的文本
        // 如果不支持文本提取，则读取器为空
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### 也可以看看

* class [Parser](../../parser)
* 命名空间 [GroupDocs.Parser](../../parser)
* 部件 [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_9}

初始化一个新的实例[`Parser`](../../parser)类[`LoadOptions`](../../../groupdocs.parser.options/loadoptions).

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| filePath | String | 文件的路径。 |
| loadOptions | LoadOptions | 打开文件的选项。 |

### 评论

**了解更多：**

* [加载特定文件格式](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [装入受密码保护的文档](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [从本地磁盘加载文档](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### 例子

文档密码由 LoadOptions 类传递：

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
    // 如果密码不正确或为空，则打印消息
    Console.WriteLine("Invalid password");
}
```

### 也可以看看

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* 命名空间 [GroupDocs.Parser](../../parser)
* 部件 [GroupDocs.Parser](../../../)

---

## Parser(string, ParserSettings) {#constructor_11}

初始化一个新的实例[`Parser`](../../parser)类[`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(string filePath, ParserSettings parserSettings)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| filePath | String | 文件的路径。 |
| parserSettings | ParserSettings | 用于自定义数据提取的解析器设置。 |

### 也可以看看

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* 命名空间 [GroupDocs.Parser](../../parser)
* 部件 [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_10}

初始化一个新的实例[`Parser`](../../parser)类[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) 和[`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| filePath | String | 文件的路径。 |
| loadOptions | LoadOptions | 打开文件的选项。 |
| parserSettings | ParserSettings | 用于自定义数据提取的解析器设置。 |

### 评论

**了解更多：**

* [加载特定文件格式](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [装入受密码保护的文档](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [记录](https://docs.groupdocs.com/display/parsernet/Logging)
* [从本地磁盘加载文档](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### 例子

以下示例显示了如何通过以下方式接收信息[`ILogger`](../../../groupdocs.parser.options/ilogger)界面：

```csharp
// 尝试
{
    // 创建 Logger 类的实例
    Logger logger = new Logger();
    // 使用解析器设置创建一个 Parser 类的实例
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
    ; // 忽略异常
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
        // 打印事件消息
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // 打印警告信息
        Console.WriteLine("Warning: " + message);
    }
}
```

### 也可以看看

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* 命名空间 [GroupDocs.Parser](../../parser)
* 部件 [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

初始化一个新的实例[`Parser`](../../parser)类.

```csharp
public Parser(Stream document)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| document | Stream | 源输入流。 |

### 评论

**了解更多：**

* [从流中加载文档](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### 例子

以下示例显示了如何从流中加载文档：

```csharp
// 使用流创建 Parser 类的实例
using (Parser parser = new Parser(stream))
{
    // 将文本提取到阅读器中
    using (TextReader reader = parser.GetText())
    {
        // 打印文档中的文本
        // 如果不支持文本提取，则读取器为空
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### 也可以看看

* class [Parser](../../parser)
* 命名空间 [GroupDocs.Parser](../../parser)
* 部件 [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

初始化一个新的实例[`Parser`](../../parser)类[`LoadOptions`](../../../groupdocs.parser.options/loadoptions).

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| document | Stream | 源输入流。 |
| loadOptions | LoadOptions | 打开文件的选项。 |

### 评论

**了解更多：**

* [加载特定文件格式](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [装入受密码保护的文档](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [从流中加载文档](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### 例子

在某些情况下有必要定义[`FileFormat`](../../../groupdocs.parser.options/fileformat) 既适用于特殊情况（数据库、电子邮件服务器），也适用于通过内容检测文件类型：

文档密码由[`LoadOptions`](../../../groupdocs.parser.options/loadoptions)班级：

```csharp
// 为 markdown 文档创建一个 Parser 类的实例
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
    // 如果密码不正确或为空，则打印消息
    Console.WriteLine("Invalid password");
}
```

### 也可以看看

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* 命名空间 [GroupDocs.Parser](../../parser)
* 部件 [GroupDocs.Parser](../../../)

---

## Parser(Stream, ParserSettings) {#constructor_7}

初始化一个新的实例[`Parser`](../../parser)类[`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(Stream document, ParserSettings parserSettings)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| document | Stream | 源输入流。 |
| parserSettings | ParserSettings | 用于自定义数据提取的解析器设置。 |

### 也可以看看

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* 命名空间 [GroupDocs.Parser](../../parser)
* 部件 [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

初始化一个新的实例[`Parser`](../../parser)类[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) 和[`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| document | Stream | 源输入流。 |
| loadOptions | LoadOptions | 打开文件的选项。 |
| parserSettings | ParserSettings | 用于自定义数据提取的解析器设置。 |

### 评论

**了解更多：**

* [加载特定文件格式](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [装入受密码保护的文档](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [从流中加载文档](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [记录](https://docs.groupdocs.com/display/parsernet/Logging)

### 例子

以下示例显示了如何通过以下方式接收信息[`ILogger`](../../../groupdocs.parser.options/ilogger)界面：

```csharp
// 尝试
{
    // 创建 Logger 类的实例
    Logger logger = new Logger();
    // 使用解析器设置创建一个 Parser 类的实例
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
    ; // 忽略异常
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
        // 打印事件消息
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // 打印警告信息
        Console.WriteLine("Warning: " + message);
    }
}
```

### 也可以看看

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* 命名空间 [GroupDocs.Parser](../../parser)
* 部件 [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

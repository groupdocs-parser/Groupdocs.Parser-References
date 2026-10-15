---
title: "パーサー"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "URI からデータを抽出するために Parsergroupdocs.parser/parser クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/groupdocs.parser/parser/parser/
---

## Parser(Uri) {#constructor_12}

[`Parser`](../../parser) クラスの新しいインスタンスを初期化し、URI からデータを抽出します。

```csharp
public Parser(Uri uri)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| uri | Uri | リクエストが送信される Uri。 |

### 関連項目

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions) {#constructor_13}

[`Parser`](../../parser) クラスの新しいインスタンスを初期化し、*loadOptions* を使用して URI からデータを抽出します。

```csharp
public Parser(Uri uri, LoadOptions loadOptions)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| uri | Uri | リクエストが送信される Uri。 |
| loadOptions | LoadOptions | ファイルを開くためのオプションです。 |

### 関連項目

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, ParserSettings) {#constructor_15}

[`Parser`](../../parser) クラスの新しいインスタンスを初期化し、*parserSettings* を使用して URI からデータを抽出します。

```csharp
public Parser(Uri uri, ParserSettings parserSettings)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| uri | Uri | リクエストが送信される Uri。 |
| parserSettings | ParserSettings | データ抽出をカスタマイズするために使用されるパーサ設定です。 |

### 関連項目

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions, ParserSettings) {#constructor_14}

[`Parser`](../../parser) クラスの新しいインスタンスを初期化し、*loadOptions* と *parserSettings* を使用して URI からデータを抽出します。

```csharp
public Parser(Uri uri, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| uri | Uri | リクエストが送信される Uri。 |
| loadOptions | LoadOptions | ファイルを開くためのオプションです。 |
| parserSettings | ParserSettings | データ抽出をカスタマイズするために使用されるパーサ設定です。 |

### 関連項目

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection) {#constructor_2}

[`Parser`](../../parser) クラスの新しいインスタンスを初期化し、データベースからデータを抽出します。

```csharp
public Parser(DbConnection connection)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| 接続 | DbConnection | データベース接続です。 |

### 備考

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### 例

次の例は、Sqlite データベースからデータを抽出する方法を示しています：

```csharp
// DbConnection オブジェクトを作成する
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// データベースからテーブルを抽出するために Parser クラスのインスタンスを作成する
using (Parser parser = new Parser(connection))
{
    // テキスト抽出がサポートされているか確認
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // 目次抽出がサポートされているか確認します
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // テーブルの一覧を取得する
    IEnumerable<TocItem> toc = parser.GetToc();
    // テーブルを反復処理する
    foreach (TocItem i in toc)
    {
        // テーブル名を出力する
        Console.WriteLine(i.Text);
        // テーブルの内容をテキストとして抽出する
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### 関連項目

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

[`Parser`](../../parser) クラスの新しいインスタンスを初期化し、データベースからデータを抽出します。

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| 接続 | DbConnection | データベース接続です。 |
| parserSettings | ParserSettings | データ抽出をカスタマイズするために使用されるパーサ設定です。 |

### 備考

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### 例

次の例は、Sqlite データベースからデータを抽出する方法を示しています：

```csharp
// DbConnection オブジェクトを作成する
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// データベースからテーブルを抽出するために Parser クラスのインスタンスを作成する
using (Parser parser = new Parser(connection))
{
    // テキスト抽出がサポートされているか確認
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // 目次抽出がサポートされているか確認します
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // テーブルの一覧を取得する
    IEnumerable<TocItem> toc = parser.GetToc();
    // テーブルを反復処理する
    foreach (TocItem i in toc)
    {
        // テーブル名を出力する
        Console.WriteLine(i.Text);
        // テーブルの内容をテキストとして抽出する
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### 関連項目

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

[`Parser`](../../parser) クラスの新しいインスタンスを初期化し、リモートメールサーバーからデータを抽出します。

```csharp
public Parser(EmailConnection connection)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| 接続 | EmailConnection | メール接続です。 |

### 備考

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### 例

次の例は、Exchange Server からメールを抽出する方法を示しています：

```csharp
// Exchange Web Services プロトコル用の接続オブジェクトを作成する
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// リモートサーバーからメールを抽出するために Parser クラスのインスタンスを作成する
using (Parser parser = new Parser(connection))
{
    // コンテナ抽出がサポートされているか確認する
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// サーバーからメールメッセージを抽出する
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // 添付ファイルを反復処理する
    foreach (ContainerItem item in emails)
    {
        // メールメッセージ用に Parser クラスのインスタンスを作成する
        using (Parser emailParser = item.OpenParser())
        {
            // メール本文を抽出する
            using (TextReader reader = emailParser.GetText())
            {
                // メール本文を出力する
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### 関連項目

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

[`Parser`](../../parser) クラスの新しいインスタンスを初期化し、リモートメールサーバーからデータを抽出します。

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| 接続 | EmailConnection | メール接続です。 |
| parserSettings | ParserSettings | データ抽出をカスタマイズするために使用されるパーサ設定です。 |

### 備考

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### 例

次の例は、Exchange Server からメールを抽出する方法を示しています：

```csharp
// Exchange Web Services プロトコル用の接続オブジェクトを作成する
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// リモートサーバーからメールを抽出するために Parser クラスのインスタンスを作成する
using (Parser parser = new Parser(connection))
{
    // コンテナ抽出がサポートされているか確認する
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// サーバーからメールメッセージを抽出する
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // 添付ファイルを反復処理する
    foreach (ContainerItem item in emails)
    {
        // メールメッセージ用に Parser クラスのインスタンスを作成する
        using (Parser emailParser = item.OpenParser())
        {
            // メール本文を抽出する
            using (TextReader reader = emailParser.GetText())
            {
                // メール本文を出力する
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### 関連項目

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_8}

[`Parser`](../../parser) クラスの新しいインスタンスを初期化します。

```csharp
public Parser(string filePath)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| filePath | 文字列 | ファイルへのパス。 |

### 備考

**Learn more:**

* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### 例

次の例はローカルディスクからドキュメントをロードする方法を示しています：

```csharp
// filePath を使用して Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // テキストをリーダーに抽出する
    using (TextReader reader = parser.GetText())
    {
        // ドキュメントからテキストを出力する
        // テキスト抽出がサポートされていない場合、リーダーは null です
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### 関連項目

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_9}

[`Parser`](../../parser) クラスの新しいインスタンスを [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) で初期化します。

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| filePath | 文字列 | ファイルへのパス。 |
| loadOptions | LoadOptions | ファイルを開くためのオプションです。 |

### 備考

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### 例

ドキュメントのパスワードは LoadOptions クラスによって渡されます：

```csharp
try
{
    // パスワードを使用して Parser クラスのインスタンスを作成します：
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // テキスト抽出がサポートされているか確認
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // ドキュメントのテキストを出力します
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // パスワードが正しくない、または空の場合にメッセージを出力します
    Console.WriteLine("Invalid password");
}
```

### 関連項目

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, ParserSettings) {#constructor_11}

[`Parser`](../../parser) クラスの新しいインスタンスを [`ParserSettings`](../../../groupdocs.parser.options/parsersettings) で初期化します。

```csharp
public Parser(string filePath, ParserSettings parserSettings)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| filePath | 文字列 | ファイルへのパス。 |
| parserSettings | ParserSettings | データ抽出をカスタマイズするために使用されるパーサ設定です。 |

### 関連項目

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_10}

[`Parser`](../../parser) クラスの新しいインスタンスを [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) と [`ParserSettings`](../../../groupdocs.parser.options/parsersettings) で初期化します。

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| filePath | 文字列 | ファイルへのパス。 |
| loadOptions | LoadOptions | ファイルを開くためのオプションです。 |
| parserSettings | ParserSettings | データ抽出をカスタマイズするために使用されるパーサ設定です。 |

### 備考

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### 例

次の例は [`ILogger`](../../../groupdocs.parser.options/ilogger) インターフェイスを介して情報を取得する方法を示しています：

```csharp
// try
{
    // Logger クラスのインスタンスを作成します
    Logger logger = new Logger();
    // parser settings を使用して Parser クラスのインスタンスを作成します
    using (Parser parser = new Parser(filePath, null, new ParserSettings(logger)))
    {
        // テキスト抽出がサポートされているか確認
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // ドキュメントのテキストを出力します
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
        // エラーメッセージを出力します
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // イベントメッセージを出力します
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // 警告メッセージを出力します
        Console.WriteLine("Warning: " + message);
    }
}
```

### 関連項目

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

[`Parser`](../../parser) クラスの新しいインスタンスを初期化します。

```csharp
public Parser(Stream document)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| ドキュメント | Stream | ソース入力ストリームです。 |

### 備考

**Learn more:**

* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### 例

次の例はストリームからドキュメントをロードする方法を示しています：

```csharp
// ストリームを使用して Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(stream))
{
    // テキストをリーダーに抽出する
    using (TextReader reader = parser.GetText())
    {
        // ドキュメントからテキストを出力する
        // テキスト抽出がサポートされていない場合、リーダーは null です
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### 関連項目

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

[`Parser`](../../parser) クラスの新しいインスタンスを [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) で初期化します。

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| ドキュメント | Stream | ソース入力ストリームです。 |
| loadOptions | LoadOptions | ファイルを開くためのオプションです。 |

### 備考

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### 例

場合によっては [`FileFormat`](../../../groupdocs.parser.options/fileformat) を定義する必要があります。特別なケース（データベース、メールサーバー）やコンテンツによるファイルタイプ検出の両方に使用します：

```csharp
// markdown ドキュメント用に Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup)))
{
    // テキスト抽出がサポートされているか確認
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    using (TextReader reader = parser.GetText())
    {
        // ドキュメントのテキストを出力します
        // Markdown が検出されました；特殊記号のないテキストが出力されます
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

ドキュメントのパスワードは [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) クラスによって渡されます：

```csharp
try
{
    // パスワードを使用して Parser クラスのインスタンスを作成します：
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // テキスト抽出がサポートされているか確認
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // ドキュメントのテキストを出力します
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // パスワードが正しくない、または空の場合にメッセージを出力します
    Console.WriteLine("Invalid password");
}
```

### 関連項目

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, ParserSettings) {#constructor_7}

[`Parser`](../../parser) クラスの新しいインスタンスを [`ParserSettings`](../../../groupdocs.parser.options/parsersettings) で初期化します。

```csharp
public Parser(Stream document, ParserSettings parserSettings)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| ドキュメント | Stream | ソース入力ストリームです。 |
| parserSettings | ParserSettings | データ抽出をカスタマイズするために使用されるパーサ設定です。 |

### 関連項目

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

[`Parser`](../../parser) クラスの新しいインスタンスを [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) と [`ParserSettings`](../../../groupdocs.parser.options/parsersettings) で初期化します。

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| ドキュメント | Stream | ソース入力ストリームです。 |
| loadOptions | LoadOptions | ファイルを開くためのオプションです。 |
| parserSettings | ParserSettings | データ抽出をカスタマイズするために使用されるパーサ設定です。 |

### 備考

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### 例

次の例は [`ILogger`](../../../groupdocs.parser.options/ilogger) インターフェイスを介して情報を取得する方法を示しています：

```csharp
// try
{
    // Logger クラスのインスタンスを作成します
    Logger logger = new Logger();
    // parser settings を使用して Parser クラスのインスタンスを作成します
    using (Parser parser = new Parser(stream, null, new ParserSettings(logger)))
    {
        // テキスト抽出がサポートされているか確認
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // ドキュメントのテキストを出力します
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
        // エラーメッセージを出力します
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // イベントメッセージを出力します
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // 警告メッセージを出力します
        Console.WriteLine("Warning: " + message);
    }
}
```

### 関連項目

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

---
title: Parser
second_title: GroupDocs.Parser for .NET API リファレンス
description: の新しいインスタンスを初期化しますParsergroupdocs.parser/parserデータベースからデータを抽出するクラス.
type: docs
weight: 10
url: /ja/net/groupdocs.parser/parser/parser/
---
## Parser(DbConnection) {#constructor_2}

の新しいインスタンスを初期化します[`Parser`](../../parser)データベースからデータを抽出するクラス.

```csharp
public Parser(DbConnection connection)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| connection | DbConnection | データベース接続。 |

### 備考

**もっと詳しく知る：**

* [データベースからデータを抽出する](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### 例

次の例は、Sqlite データベースからデータを抽出する方法を示しています。

```csharp
// DbConnection オブジェクトを作成します
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// データベースからテーブルを抽出する Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(connection))
{
    // テキスト抽出がサポートされているかどうかを確認します
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // toc 抽出がサポートされているかどうかを確認します
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // テーブルのリストを取得
    IEnumerable<TocItem> toc = parser.GetToc();
    // テーブルを繰り返します
    foreach (TocItem i in toc)
    {
        // テーブル名を表示
        Console.WriteLine(i.Text);
        // 表の内容をテキストとして抽出します
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### 関連項目

* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

の新しいインスタンスを初期化します[`Parser`](../../parser)データベースからデータを抽出するクラス.

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| connection | DbConnection | データベース接続。 |
| parserSettings | ParserSettings | データ抽出のカスタマイズに使用されるパーサー設定。 |

### 備考

**もっと詳しく知る：**

* [データベースからデータを抽出する](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [ロギング](https://docs.groupdocs.com/display/parsernet/Logging)

### 例

次の例は、Sqlite データベースからデータを抽出する方法を示しています。

```csharp
// DbConnection オブジェクトを作成します
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// データベースからテーブルを抽出する Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(connection))
{
    // テキスト抽出がサポートされているかどうかを確認します
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // toc 抽出がサポートされているかどうかを確認します
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // テーブルのリストを取得
    IEnumerable<TocItem> toc = parser.GetToc();
    // テーブルを繰り返します
    foreach (TocItem i in toc)
    {
        // テーブル名を表示
        Console.WriteLine(i.Text);
        // 表の内容をテキストとして抽出します
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
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

の新しいインスタンスを初期化します[`Parser`](../../parser)リモート電子メール サーバーからデータを抽出するクラス.

```csharp
public Parser(EmailConnection connection)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| connection | EmailConnection | メール接続。 |

### 備考

**もっと詳しく知る：**

* [POP、IMAP、または Exchange Web サービス プロトコルを介してリモート サーバーから電子メールを抽出します。](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### 例

次の例は、Exchange Server から電子メールを抽出する方法を示しています。

```csharp
// Exchange Web サービス プロトコルの接続オブジェクトを作成します 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Parser クラスのインスタンスを作成して、リモート サーバーから電子メールを抽出します
using (Parser parser = new Parser(connection))
{
    // コンテナの抽出がサポートされているかどうかを確認します
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// サーバーから電子メール メッセージを抽出します
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // 添付ファイルを繰り返す
    foreach (ContainerItem item in emails)
    {
        // 電子メール メッセージの Parser クラスのインスタンスを作成します
        using (Parser emailParser = item.OpenParser())
        {
            // メール本文を抽出する
            using (TextReader reader = emailParser.GetText())
            {
                // メール本文を印刷する
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### 関連項目

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

の新しいインスタンスを初期化します[`Parser`](../../parser)リモート電子メール サーバーからデータを抽出するクラス.

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| connection | EmailConnection | メール接続。 |
| parserSettings | ParserSettings | データ抽出のカスタマイズに使用されるパーサー設定。 |

### 備考

**もっと詳しく知る：**

* [POP、IMAP、または Exchange Web サービス プロトコルを介してリモート サーバーから電子メールを抽出します。](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [ロギング](https://docs.groupdocs.com/display/parsernet/Logging)

### 例

次の例は、Exchange Server から電子メールを抽出する方法を示しています。

```csharp
// Exchange Web サービス プロトコルの接続オブジェクトを作成します 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Parser クラスのインスタンスを作成して、リモート サーバーから電子メールを抽出します
using (Parser parser = new Parser(connection))
{
    // コンテナの抽出がサポートされているかどうかを確認します
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// サーバーから電子メール メッセージを抽出します
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // 添付ファイルを繰り返す
    foreach (ContainerItem item in emails)
    {
        // 電子メール メッセージの Parser クラスのインスタンスを作成します
        using (Parser emailParser = item.OpenParser())
        {
            // メール本文を抽出する
            using (TextReader reader = emailParser.GetText())
            {
                // メール本文を印刷する
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
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_8}

の新しいインスタンスを初期化します[`Parser`](../../parser)class.

```csharp
public Parser(string filePath)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| filePath | String | ファイルへのパス。 |

### 備考

**もっと詳しく知る：**

* [ドキュメントをローカル ディスクから読み込む](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### 例

次の例は、ローカル ディスクからドキュメントをロードする方法を示しています。

```csharp
// filePath を使用して Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // テキストをリーダーに抽出します
    using (TextReader reader = parser.GetText())
    {
        // ドキュメントからテキストを出力します
        // テキスト抽出がサポートされていない場合、リーダーは null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### 関連項目

* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_9}

の新しいインスタンスを初期化します[`Parser`](../../parser)クラス[`LoadOptions`](../../../groupdocs.parser.options/loadoptions).

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| filePath | String | ファイルへのパス。 |
| loadOptions | LoadOptions | ファイルを開くためのオプション。 |

### 備考

**もっと詳しく知る：**

* [特定のファイル形式の読み込み](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [パスワードで保護されたドキュメントの読み込み](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [ドキュメントをローカル ディスクから読み込む](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### 例

ドキュメントのパスワードは LoadOptions クラスによって渡されます。

```csharp
try
{
    // パスワードを使用して Parser クラスのインスタンスを作成します。
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // テキスト抽出がサポートされているかどうかを確認します
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // ドキュメントのテキストを印刷する
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // パスワードが正しくないか空の場合はメッセージを出力します
    Console.WriteLine("Invalid password");
}
```

### 関連項目

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

---

## Parser(string, ParserSettings) {#constructor_11}

の新しいインスタンスを初期化します[`Parser`](../../parser)クラス[`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(string filePath, ParserSettings parserSettings)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| filePath | String | ファイルへのパス。 |
| parserSettings | ParserSettings | データ抽出のカスタマイズに使用されるパーサー設定。 |

### 関連項目

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_10}

の新しいインスタンスを初期化します[`Parser`](../../parser)クラス[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) と[`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| filePath | String | ファイルへのパス。 |
| loadOptions | LoadOptions | ファイルを開くためのオプション。 |
| parserSettings | ParserSettings | データ抽出のカスタマイズに使用されるパーサー設定。 |

### 備考

**もっと詳しく知る：**

* [特定のファイル形式の読み込み](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [パスワードで保護されたドキュメントの読み込み](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [ロギング](https://docs.groupdocs.com/display/parsernet/Logging)
* [ドキュメントをローカル ディスクから読み込む](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### 例

次の例は、次の方法で情報を受け取る方法を示しています。[`ILogger`](../../../groupdocs.parser.options/ilogger)インターフェース：

```csharp
// 試す
{
    // Logger クラスのインスタンスを作成します
    Logger logger = new Logger();
    // パーサー設定で Parser クラスのインスタンスを作成します
    using (Parser parser = new Parser(filePath, null, new ParserSettings(logger)))
    {
        // テキスト抽出がサポートされているかどうかを確認します
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // ドキュメントのテキストを印刷する
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // 例外を無視
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // エラーメッセージを表示
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // イベントメッセージを出力
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // 警告メッセージを表示
        Console.WriteLine("Warning: " + message);
    }
}
```

### 関連項目

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

の新しいインスタンスを初期化します[`Parser`](../../parser)class.

```csharp
public Parser(Stream document)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| document | Stream | ソース入力ストリーム。 |

### 備考

**もっと詳しく知る：**

* [ストリームからドキュメントをロード](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### 例

次の例は、ストリームからドキュメントをロードする方法を示しています。

```csharp
// ストリームで Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(stream))
{
    // テキストをリーダーに抽出します
    using (TextReader reader = parser.GetText())
    {
        // ドキュメントからテキストを出力します
        // テキスト抽出がサポートされていない場合、リーダーは null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### 関連項目

* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

の新しいインスタンスを初期化します[`Parser`](../../parser)クラス[`LoadOptions`](../../../groupdocs.parser.options/loadoptions).

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| document | Stream | ソース入力ストリーム。 |
| loadOptions | LoadOptions | ファイルを開くためのオプション。 |

### 備考

**もっと詳しく知る：**

* [特定のファイル形式の読み込み](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [パスワードで保護されたドキュメントの読み込み](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [ストリームからドキュメントをロード](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### 例

場合によっては、定義する必要があります[`FileFormat`](../../../groupdocs.parser.options/fileformat) 特殊なケース (データベース、電子メール サーバー) とコンテンツによるファイル タイプの検出の両方:

ドキュメントパスワードが渡されます[`LoadOptions`](../../../groupdocs.parser.options/loadoptions)クラス：

```csharp
// マークダウン ドキュメントの Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup)))
{
    // テキスト抽出がサポートされているかどうかを確認します
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    using (TextReader reader = parser.GetText())
    {
        // ドキュメントのテキストを印刷する
        // マークダウンが検出されました。特殊記号のないテキストが印刷されます
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

```csharp
try
{
    // パスワードを使用して Parser クラスのインスタンスを作成します。
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // テキスト抽出がサポートされているかどうかを確認します
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // ドキュメントのテキストを印刷する
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // パスワードが正しくないか空の場合はメッセージを出力します
    Console.WriteLine("Invalid password");
}
```

### 関連項目

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

---

## Parser(Stream, ParserSettings) {#constructor_7}

の新しいインスタンスを初期化します[`Parser`](../../parser)クラス[`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(Stream document, ParserSettings parserSettings)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| document | Stream | ソース入力ストリーム。 |
| parserSettings | ParserSettings | データ抽出のカスタマイズに使用されるパーサー設定。 |

### 関連項目

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

の新しいインスタンスを初期化します[`Parser`](../../parser)クラス[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) と[`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| document | Stream | ソース入力ストリーム。 |
| loadOptions | LoadOptions | ファイルを開くためのオプション。 |
| parserSettings | ParserSettings | データ抽出のカスタマイズに使用されるパーサー設定。 |

### 備考

**もっと詳しく知る：**

* [特定のファイル形式の読み込み](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [パスワードで保護されたドキュメントの読み込み](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [ストリームからドキュメントをロード](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [ロギング](https://docs.groupdocs.com/display/parsernet/Logging)

### 例

次の例は、次の方法で情報を受け取る方法を示しています。[`ILogger`](../../../groupdocs.parser.options/ilogger)インターフェース：

```csharp
// 試す
{
    // Logger クラスのインスタンスを作成します
    Logger logger = new Logger();
    // パーサー設定で Parser クラスのインスタンスを作成します
    using (Parser parser = new Parser(stream, null, new ParserSettings(logger)))
    {
        // テキスト抽出がサポートされているかどうかを確認します
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // ドキュメントのテキストを印刷する
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // 例外を無視
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // エラーメッセージを表示
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // イベントメッセージを出力
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // 警告メッセージを表示
        Console.WriteLine("Warning: " + message);
    }
}
```

### 関連項目

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

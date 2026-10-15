---
title: "GetText"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ドキュメントからテキストを抽出します。"
type: docs
weight: 180
url: /ja/net/groupdocs.parser/parser/gettext/
---

## GetText() {#gettext}

ドキュメントからテキストを抽出します。

```csharp
public TextReader GetText()
```

### 戻り値

抽出されたテキストを持つ TextReader クラスのインスタンスです。テキスト抽出がサポートされていない場合は `null` です。

### 備考

**Learn more:**

* [Extract text from documents](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### 例

以下の例は、ドキュメントからテキストを抽出する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using(Parser parser = new Parser(filePath))
{
    // テキストをリーダーに抽出する
    using(TextReader reader = parser.GetText())
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

## GetText(TextOptions) {#gettext_1}

生の高速テキスト抽出モードを有効にするテキストオプションを使用して、ドキュメントからテキストページを抽出します。

```csharp
public TextReader GetText(TextOptions options)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| options | TextOptions | テキスト抽出オプションです。 |

### 戻り値

抽出されたテキストを持つ TextReader クラスのインスタンスです。テキスト抽出がサポートされていない場合は `null` です。

### 備考

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### 例

次の例は、ドキュメントから生テキストを抽出する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using(Parser parser = new Parser(filePath))
{
    // リーダーに生テキストを抽出する
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // ドキュメントからテキストを出力する
        // テキスト抽出がサポートされていない場合、リーダーは null です
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### 関連項目

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

ドキュメントページからテキストを抽出します。

```csharp
public TextReader GetText(int pageIndex)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| pageIndex | Int32 | 0 から始まるページインデックスです。 |

### 戻り値

抽出されたテキストを持つ TextReader クラスのインスタンス; テキストページ抽出がサポートされていない場合は `null`。

### 備考

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### 例

次の例は、ドキュメントページからテキストを抽出する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using(Parser parser = new Parser(filePath))
{
    // ドキュメントがテキスト抽出をサポートしているか確認する
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // ドキュメント情報を取得する
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // ドキュメントにページがあるか確認する
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // ページを反復処理する
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // ページ番号を出力する
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // テキストをリーダーに抽出する
        using(TextReader reader = parser.GetText(p))
        {
            // ドキュメントからテキストを出力する
            // テキスト抽出機能のサポートを事前に確認したため、null チェックは無視します
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

## GetText(int, TextOptions) {#gettext_3}

テキストオプションを使用してドキュメントページからテキストを抽出します（生の高速テキスト抽出モードを有効にするため）。

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| pageIndex | Int32 | 0 から始まるページインデックスです。 |
| options | TextOptions | テキスト抽出オプションです。 |

### 戻り値

抽出されたテキストを持つ TextReader クラスのインスタンス; テキストページ抽出がサポートされていない場合は `null`。

### 備考

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### 例

次の例は、ドキュメントページから生テキストを抽出する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using(Parser parser = new Parser(filePath))
{
    // ドキュメントがテキスト抽出をサポートしているか確認する
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // ドキュメント情報を取得する
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // ドキュメントにページがあるか確認する
    if(documentInfo == null || documentInfo.RawPageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // ページを反復処理する
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // ページ番号を出力する
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // テキストをリーダーに抽出する
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // ドキュメントからテキストを出力する
            // テキスト抽出機能のサポートを事前に確認したため、null チェックは無視します
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### 関連項目

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

---
title: "GetFormattedText"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ドキュメントから書式付きテキストを抽出します。"
type: docs
weight: 100
url: /ja/net/groupdocs.parser/parser/getformattedtext/
---

## GetFormattedText(FormattedTextOptions) {#getformattedtext}

ドキュメントから書式付きテキストを抽出します。

```csharp
public TextReader GetFormattedText(FormattedTextOptions options)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| options | FormattedTextOptions | 書式化テキスト抽出オプションです。 |

### 戻り値

抽出されたテキストを持つ TextReader クラスのインスタンスです；書式化テキスト抽出がサポートされていない場合は `null`。

### 備考

**Learn more:**

* [Extract formatted text from document](https://docs.groupdocs.com/display/parsernet/Extract+formatted+text+from+document)
* Extract a document text as [HTML](https://docs.groupdocs.com/display/parsernet/HTML)
* Extract a document text as [Markdown](https://docs.groupdocs.com/display/parsernet/Markdown)
* Extract a document text as [Plain text](https://docs.groupdocs.com/display/parsernet/Plain+text)

### 例

以下の例は、ドキュメントのテキストを HTML テキストとして抽出する方法を示しています：

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // 書式化テキストをリーダーに抽出する
    using (TextReader reader = parser.GetFormattedText(new FormattedTextOptions(FormattedTextMode.Html)))
    {
        // ドキュメントから書式化テキストを出力する
        // 書式化テキスト抽出がサポートされていない場合、リーダーは null です
        Console.WriteLine(reader == null ? "Formatted text extraction isn't suppported" : reader.ReadToEnd());
    }
}
```

### 関連項目

* class [FormattedTextOptions](../../../groupdocs.parser.options/formattedtextoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetFormattedText(int, FormattedTextOptions) {#getformattedtext_1}

ドキュメントページから書式付きテキストを抽出します。

```csharp
public TextReader GetFormattedText(int pageIndex, FormattedTextOptions options)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| pageIndex | Int32 | 0 から始まるページインデックスです。 |
| options | FormattedTextOptions | 書式化テキスト抽出オプションです。 |

### 戻り値

抽出されたテキストを持つ TextReader クラスのインスタンスです；書式化テキストページ抽出がサポートされていない場合は `null`。

### 備考

**Learn more:**

* [Extract formatted text from document page](https://docs.groupdocs.com/display/parsernet/Extract+formatted+text+from+document+page)
* Extract a document text as [HTML](https://docs.groupdocs.com/display/parsernet/HTML)
* Extract a document text as [Markdown](https://docs.groupdocs.com/display/parsernet/Markdown)
* Extract a document text as [Plain text](https://docs.groupdocs.com/display/parsernet/Plain+text)

### 例

以下の例は、ドキュメントページのテキストを Markdown テキストとして抽出する方法を示しています：

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // ドキュメントが書式化テキスト抽出をサポートしているか確認する
    if (!parser.Features.FormattedText)
    {
        Console.WriteLine("Document isn't supports formatted text extraction.");
        return;
    }
    
    // ドキュメント情報を取得する
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // ドキュメントにページがあるか確認する
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // ページを反復処理する
    for (int p = 0; p<documentInfo.PageCount; p++)
    {
        // ページ番号を出力する
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
        // 書式化テキストをリーダーに抽出する
        using (TextReader reader = parser.GetFormattedText(p, new FormattedTextOptions(FormattedTextMode.Markdown)))
        {
            // ドキュメントから書式化テキストを出力する
            // 以前に書式化テキスト抽出機能のサポートを確認したので、null チェックは無視します
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### 関連項目

* class [FormattedTextOptions](../../../groupdocs.parser.options/formattedtextoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

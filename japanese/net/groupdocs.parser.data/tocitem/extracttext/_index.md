---
title: "ExtractText"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "TocItemgroupdocs.parser.data/tocitem オブジェクトが参照するドキュメントからテキストを抽出します。"
type: docs
weight: 50
url: /ja/net/groupdocs.parser.data/tocitem/extracttext/
---

## TocItem.ExtractText method

[`TocItem`](../../tocitem) オブジェクトが参照するドキュメントからテキストを抽出します。

```csharp
public virtual TextReader ExtractText()
```

### 戻り値

抽出されたテキストを持つ TextReader クラスのインスタンスです。

### 例

以下は目次項目を使用してテキストを抽出する例です。

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(Constants.SampleDocxWithToc))
{
    // 目次を取得します
    IEnumerable<TocItem> tocItems = parser.GetToc();
    // 目次抽出がサポートされているか確認します
    if (tocItems == null)
    {
        Console.WriteLine("Table of contents extraction isn't supported");
    }
    // 項目を反復処理します
    foreach (TocItem tocItem in tocItems)
    {
        // 章のテキストを出力します
        using (TextReader reader = tocItem.ExtractText())
        {
            Console.WriteLine("----");
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### 関連項目

* class [TocItem](../../tocitem)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

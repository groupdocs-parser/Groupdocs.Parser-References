---
title: "GetToc"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ドキュメントから目次を抽出します。"
type: docs
weight: 200
url: /ja/net/groupdocs.parser/parser/gettoc/
---

## Parser.GetToc method

ドキュメントから目次を抽出します。

```csharp
public IEnumerable<TocItem> GetToc()
```

### 戻り値

目次抽出がサポートされていない場合は `null`、それ以外は目次項目のコレクションです。

### 備考

**Learn more:**

* [Extract table of contents](https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents)
* [Extract text by table of contents item](https://docs.groupdocs.com/display/parsernet/Extract+text+by+table+of+contents+item)
* [Extract table of contents from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents+from+Microsoft+Office+Word+documents)
* [Extract table of contents from EPUB eBooks](https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents+from+EPUB+eBooks)

### 例

次の例は CHM ファイルから目次を抽出する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
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
 
    // 目次を取得します
    IEnumerable<TocItem> toc = parser.GetToc();
    
    // 項目を反復処理します
    foreach (TocItem i in toc)
    {
        // 目次テキストを印刷する
        Console.WriteLine(i.Text);
        // ページインデックスに値があるか確認する
        if (i.PageIndex == null)
        {
            continue;
        }
        // ページテキストを抽出する
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### 関連項目

* class [TocItem](../../../groupdocs.parser.data/tocitem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

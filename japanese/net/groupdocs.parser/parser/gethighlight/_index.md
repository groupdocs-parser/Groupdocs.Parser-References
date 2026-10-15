---
title: "GetHighlight"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ドキュメントからハイライトを抽出します。"
type: docs
weight: 110
url: /ja/net/groupdocs.parser/parser/gethighlight/
---

## Parser.GetHighlight method

ドキュメントからハイライトを抽出します。

```csharp
public HighlightItem GetHighlight(int position, bool isDirect, HighlightOptions options)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| 位置 | Int32 | ハイライトの開始位置です。 |
| isDirect | Boolean | ハイライト抽出が直接かどうかを示す値です。`true` はハイライトが *position* の右側から抽出された場合を示し、そうでなければ `false` です。 |
| options | HighlightOptions | ハイライト抽出オプションです。 |

### 戻り値

抽出されたハイライトを表す [`HighlightItem`](../../../groupdocs.parser.data/highlightitem) クラスのインスタンスです。ハイライト抽出がサポートされていない場合は `null` です。

### 備考

**Learn more:**

* [Extract highlights](https://docs.groupdocs.com/display/parsernet/Extract+highlights)

### 例

以下の例は、3語を含むハイライトを抽出する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // ハイライトを抽出:
    HighlightItem hl = parser.GetHighlight(2, true, new HighlightOptions(3));
    
    // ハイライト抽出がサポートされているか確認する
    if (hl == null)
    {
        Console.WriteLine("Highlight extraction isn't supported");
        return;
    }
    
    // 抽出されたハイライトを出力する
    Console.WriteLine(string.Format("At {0}: {1}", hl.Position, hl.Text));
}
```

### 関連項目

* class [HighlightItem](../../../groupdocs.parser.data/highlightitem)
* class [HighlightOptions](../../../groupdocs.parser.options/highlightoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

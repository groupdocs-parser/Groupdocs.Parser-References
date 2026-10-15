---
title: "RawPageCount"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ドキュメントの生ページ総数を取得します。"
type: docs
weight: 40
url: /ja/net/groupdocs.parser.options/documentinfo/rawpagecount/
---

## DocumentInfo.RawPageCount property

ドキュメントの生ページ総数を取得します。

```csharp
public int RawPageCount { get; }
```

### Property Value

生ページの総数を表す整数値です。

### 備考

生テキスト抽出には `RawPageCount` プロパティを使用し、[`PageCount`](../pagecount) プロパティの代わりに使用してください。正確な抽出モードと生テキスト抽出モードでは、ドキュメントによってページ番号が異なる場合があります。[`PageCount`](../pagecount) プロパティは余分な計算を行う可能性があり、生モードでのテキスト抽出速度に影響します。

### 関連項目

* class [DocumentInfo](../../documentinfo)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

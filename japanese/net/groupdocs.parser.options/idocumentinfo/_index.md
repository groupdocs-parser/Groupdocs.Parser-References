---
title: "IDocumentInfo"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ドキュメント情報を表します。"
type: docs
weight: 370
url: /ja/net/groupdocs.parser.options/idocumentinfo/
---

## IDocumentInfo interface

ドキュメント情報を表します。

```csharp
public interface IDocumentInfo
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [FileType](../../groupdocs.parser.options/idocumentinfo/filetype) { get; } | ドキュメントのタイプを取得します。 |
| [PageCount](../../groupdocs.parser.options/idocumentinfo/pagecount) { get; } | ドキュメントの総ページ数を取得します。 |
| [Pages](../../groupdocs.parser.options/idocumentinfo/pages) { get; } | インデックスやページサイズなど、ページに関する情報を取得します。 |
| [RawPageCount](../../groupdocs.parser.options/idocumentinfo/rawpagecount) { get; } | ドキュメントの生ページ総数を取得します。 |
| [Size](../../groupdocs.parser.options/idocumentinfo/size) { get; } | ドキュメントのサイズ（バイト単位）を取得します。 |

### 備考

このインターフェイスを実装するオブジェクトは、[`GetDocumentInfo`](../../groupdocs.parser/parser/getdocumentinfo) メソッドによって返されます。使用例はそちらをご覧ください。**詳しく見る:**

* [Get document info](https://docs.groupdocs.com/display/parsernet/Get+document+info)
* [Detect encoding](https://docs.groupdocs.com/display/parsernet/Detect+encoding)

### 関連項目

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

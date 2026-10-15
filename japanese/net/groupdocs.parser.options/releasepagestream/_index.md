---
title: "ReleasePageStream"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "CreatePageStream によって作成されたストリームを解放するメソッドを表します。/createpagestream デリゲート。"
type: docs
weight: 580
url: /ja/net/groupdocs.parser.options/releasepagestream/
---

## ReleasePageStream delegate

[`CreatePageStream`](../createpagestream) デリゲートによって作成されたストリームを解放するメソッドを表します。

```csharp
public delegate void ReleasePageStream(int pageNumber, Stream pageStream);
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| pageNumber | Int32 | 生成されたページプレビューのページ番号です。 |
| pageStream | Stream | 生成されたページプレビューを含むストリームです。 |

### 関連項目

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

---
title: ReleasePageStream
second_title: GroupDocs.Parser for .NET API リファレンス
description: によって作成されたストリームを解放するメソッドを表しますCreatePageStream./createpagestreamデリゲート
type: docs
weight: 600
url: /ja/net/groupdocs.parser.options/releasepagestream/
---
## ReleasePageStream delegate

によって作成されたストリームを解放するメソッドを表します[`CreatePageStream`](../createpagestream)デリゲート。

```csharp
public delegate void ReleasePageStream(int pageNumber, Stream pageStream);
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| pageNumber | Int32 | 生成されたページ プレビューのページ番号。 |
| pageStream | Stream | 生成されたページ プレビューを含むストリーム。 |

### 関連項目

* 名前空間 [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* 組み立て [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

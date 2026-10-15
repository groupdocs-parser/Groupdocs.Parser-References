---
title: "PreviewOptions"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "出力ストリームが閉じられるように、PreviewOptionsgroupdocs.parser.options/previewoptions クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/groupdocs.parser.options/previewoptions/previewoptions/
---

## PreviewOptions(CreatePageStream) {#constructor}

出力ストリームが閉じられるように、[`PreviewOptions`](../../previewoptions) クラスの新しいインスタンスを初期化します。

```csharp
public PreviewOptions(CreatePageStream createPageStream)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| createPageStream | CreatePageStream | 特定のページプレビュー用のストリームを作成します。 |

### 関連項目

* delegate [CreatePageStream](../../createpagestream)
* class [PreviewOptions](../../previewoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PreviewOptions(CreatePageStream, ReleasePageStream) {#constructor_1}

出力ストリームがクライアントに返され、さらに使用できるように、[`PreviewOptions`](../../previewoptions) クラスの新しいインスタンスを初期化します。

```csharp
public PreviewOptions(CreatePageStream createPageStream, ReleasePageStream releasePageStream)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| createPageStream | CreatePageStream | 特定のページプレビュー用のストリームを作成します |
| releasePageStream | ReleasePageStream | ページプレビューの生成が完了したことを通知し、出力ストリームを取得します。 |

### 関連項目

* delegate [CreatePageStream](../../createpagestream)
* delegate [ReleasePageStream](../../releasepagestream)
* class [PreviewOptions](../../previewoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

---
title: "Metadata"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "メタデータ アイテムのコレクションを取得します。"
type: docs
weight: 30
url: /ja/net/groupdocs.parser.data/containeritem/metadata/
---

## ContainerItem.Metadata property

メタデータ アイテムのコレクションを取得します。

```csharp
public IEnumerable<MetadataItem> Metadata { get; }
```

### Property Value

メタデータが設定されていない場合は空の、[`MetadataItem`](../../metadataitem) オブジェクトのコレクション。

### 備考

これらのメタデータはドキュメントではなくコンテナ要素自体を指します。コンテナの種類に応じて、メタデータには以下の項目が含まれる場合があります：

**Email Attachments**

**Name**

**Description**

**content-type**

添付コンテンツの MIME タイプ。

**ZIP Archives**

**Name**

**Description**

**date**

Zip エントリで示されるファイルが最終更新された日時。

**disposition**

画像添付がインラインかどうかを検出するには、'disposition' メタデータを使用します。存在する場合、'inline' または 'attachment' の値を取ります。

**Outlook Storage**

**Name**

**Description**

**date**

Outlook ストレージ項目が最終更新された日時。

**email-sender**

「sender」フィールドの値。

**email-to**

「to」フィールドの値。

**subject**

「subject」フィールドの値。

### 関連項目

* class [MetadataItem](../../metadataitem)
* class [ContainerItem](../../containeritem)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

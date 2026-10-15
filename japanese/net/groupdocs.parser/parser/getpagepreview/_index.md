---
title: "GetPagePreview"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ドキュメントページのプレビューを生成します。"
type: docs
weight: 150
url: /ja/net/groupdocs.parser/parser/getpagepreview/
---

## GetPagePreview(int) {#getpagepreview}

ドキュメントページのプレビューを生成します。

```csharp
public Stream GetPagePreview(int pageIndex)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| pageIndex | Int32 | 0 から始まるページインデックスです。 |

### 戻り値

ドキュメントページの画像を含む Stream のインスタンスです。ページプレビュー生成がサポートされていない場合は `null` になります。

### 関連項目

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetPagePreview(int, PagePreviewOptions) {#getpagepreview_1}

カスタマイズオプションを使用して、ドキュメントページのプレビューを生成します。

```csharp
public Stream GetPagePreview(int pageIndex, PagePreviewOptions options)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| pageIndex | Int32 | 0 から始まるページインデックスです。 |
| options | PagePreviewOptions | プレビュー生成をカスタマイズするためのオプションです。 |

### 戻り値

ドキュメントページの画像を含む Stream のインスタンスです。ページプレビュー生成がサポートされていない場合は `null` になります。

### 関連項目

* class [PagePreviewOptions](../../../groupdocs.parser.options/pagepreviewoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

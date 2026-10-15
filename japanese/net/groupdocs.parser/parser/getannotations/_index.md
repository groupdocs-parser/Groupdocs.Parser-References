---
title: "GetAnnotations"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ドキュメントから注釈を抽出します。現在、PDF 形式のみがサポートされていることに注意してください。"
type: docs
weight: 60
url: /ja/net/groupdocs.parser/parser/getannotations/
---

## GetAnnotations() {#getannotations}

ドキュメントから注釈を抽出します。現在、PDF 形式のみがサポートされていることに注意してください。

```csharp
public IEnumerable<AnnotationItem> GetAnnotations()
```

### 戻り値

注釈項目のコレクションです。注釈抽出がサポートされていない場合は `null` になります。

### 関連項目

* class [AnnotationItem](../../../groupdocs.parser.data/annotationitem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetAnnotations(int) {#getannotations_1}

ドキュメントページから注釈を抽出します。現在、PDF 形式のみがサポートされていることに注意してください。

```csharp
public IEnumerable<AnnotationItem> GetAnnotations(int pageIndex)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| pageIndex | Int32 | 0 から始まるページインデックスです。 |

### 戻り値

注釈項目のコレクションです。注釈抽出がサポートされていない場合は `null` になります。

### 関連項目

* class [AnnotationItem](../../../groupdocs.parser.data/annotationitem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

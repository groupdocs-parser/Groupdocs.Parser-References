---
title: "テンプレート"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "Templategroupdocs.parser.templates/template クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/groupdocs.parser.templates/template/template/
---

## Template(IEnumerable&lt;TemplateItem&gt;) {#constructor}

[`Template`](../../template) クラスの新しいインスタンスを初期化します。

```csharp
public Template(IEnumerable<TemplateItem> items)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| items | IEnumerable`1 | [`TemplateItem`](../../templateitem) オブジェクトのコレクションです。 |

### 例

使用方法:

```csharp
// テンプレート フィールドの配列を作成します。
TemplateItem[] fields = new TemplateItem[]
{
   new TemplateField(new TemplateRegexPosition("From"), "From", 0),
   new TemplateField(
       new TemplateLinkedPosition("From", new Size(100, 10), new TemplateLinkedPositionEdges(false, false, false, true)),
       "FromCompany",
       0),
   new TemplateField(
       new TemplateLinkedPosition("FromCompany", new Size(100, 30), new TemplateLinkedPositionEdges(false, false, false, true)),
       "FromAddress",
       0)
};

// ドキュメントテンプレートを作成
Template template = new Template(fields);
```

### 関連項目

* class [TemplateItem](../../templateitem)
* class [Template](../../template)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## Template(IEnumerable&lt;TemplateItem&gt;, TemplateOptions) {#constructor_1}

[`Template`](../../template) クラスをテンプレート オプションとともに新しいインスタンスとして初期化します。

```csharp
public Template(IEnumerable<TemplateItem> items, TemplateOptions options)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| items | IEnumerable`1 | [`TemplateItem`](../../templateitem) オブジェクトのコレクションです。 |
| options | TemplateOptions | テンプレート オプションです。 |

### 関連項目

* class [TemplateItem](../../templateitem)
* class [TemplateOptions](../../templateoptions)
* class [Template](../../template)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

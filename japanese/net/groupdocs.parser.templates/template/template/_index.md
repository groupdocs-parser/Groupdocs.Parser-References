---
title: Template
second_title: GroupDocs.Parser for .NET API リファレンス
description: の新しいインスタンスを初期化しますTemplategroupdocs.parser.templates/templateclass.
type: docs
weight: 10
url: /ja/net/groupdocs.parser.templates/template/template/
---
## Template constructor

の新しいインスタンスを初期化します[`Template`](../../template)class.

```csharp
public Template(IEnumerable<TemplateItem> items)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| items | IEnumerable`1 | のコレクション[`TemplateItem`](../../templateitem)オブジェクト。 |

### 例

使用法：

```csharp
// テンプレート フィールドの配列を作成します
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

// ドキュメント テンプレートを作成します
Template template = new Template(fields);
```

### 関連項目

* class [TemplateItem](../../templateitem)
* class [Template](../../template)
* 名前空間 [GroupDocs.Parser.Templates](../../template)
* 組み立て [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

---
title: "TryParse"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "エッジの文字列表現をクラスの等価物に変換します。戻り値は変換が成功したか失敗したかを示します。"
type: docs
weight: 90
url: /ja/net/groupdocs.parser.templates/templatelinkedpositionedges/tryparse/
---

## TemplateLinkedPositionEdges.TryParse method

エッジの文字列表現をクラスの等価物に変換します。戻り値は変換が成功したか失敗したかを示します。

```csharp
public static bool TryParse(string s, out TemplateLinkedPositionEdges edges)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| s | 文字列 | 変換するエッジを含む文字列。 |
| edges | TemplateLinkedPositionEdges& | メソッドが戻ると、変換が成功した場合はパラメータ *s* で指定された値に相当する [`TemplateLinkedPositionEdges`](../../templatelinkedpositionedges) クラスのインスタンスが含まれ、そうでない場合は `null` になります。 |

### 戻り値

*s* が正常に変換された場合は `true`、それ以外の場合は `false` です。

### 関連項目

* class [TemplateLinkedPositionEdges](../../templatelinkedpositionedges)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

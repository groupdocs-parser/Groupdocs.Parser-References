---
title: "PageArea"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "フィールドの値を取得します。"
type: docs
weight: 30
url: /ja/net/groupdocs.parser.data/fielddata/pagearea/
---

## FieldData.PageArea property

フィールドの値を取得します。

```csharp
public PageArea PageArea { get; }
```

### Property Value

フィールドの値を表す[`PageArea`](../../pagearea)クラスのインスタンスです。

### 例

フィールドの `PageArea` プロパティは、[`PageArea`](../../pagearea) クラスの継承クラスのいずれかを含む可能性があります。例えば、[`ParseForm`](../../../groupdocs.parser/parser/parseform) メソッドはテキストフィールドのみを抽出します。

```csharp
// フィールドデータを取得する
FieldData field = data[i];
// フィールドデータにテキストが含まれているか確認する
if(field.PageArea is PageTextArea)
{
    // フィールドテキストの値を出力する
    Console.WriteLine(field.Text);
}
```

### 関連項目

* class [PageArea](../../pagearea)
* class [FieldData](../../fielddata)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

---
title: "項目"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "インデックスでフィールドデータを取得します。"
type: docs
weight: 20
url: /ja/net/groupdocs.parser.data/documentdata/item/
---

## DocumentData indexer

インデックスでフィールドデータを取得します。

```csharp
public FieldData this[int index] { get; }
```

| Parameter | 説明 |
| --- | --- |
| index | フィールドのゼロベースインデックスです。 |

### 戻り値

[`FieldData`](../../fielddata) クラスのインスタンスです。

### 例

すべてのフィールドを反復処理:

```csharp
for (int i = 0; i < data.Count; i++)
{
    Console.Write(data[i].Name + ": ");
    PageTextArea area = data[i].PageArea as PageTextArea;
    Console.WriteLine(area == null ? "Not a template field" : area.Text);
}
```

[`FieldData`](../../fielddata) class represents field data. Depending on the field [`PageArea`](../../fielddata/pagearea) property can contain any of the inheritors of [`PageArea`](../../pagearea) class. For example, [`ParseForm`](../../../groupdocs.parser/parser/parseform) method extracts only text fields:

```csharp
// パーサーを作成する
using (Parser parser = new Parser(filePath))
{
    // PDF フォームからデータを抽出する
    DocumentData data = parser.ParseForm();
    // 抽出されたフィールドを反復処理する
    for (int i = 0; i < data.Count; i++)
    {
        // 抽出されたフィールドを取得する
        FieldData field = data[i];
        // フィールド名を出力する
        Console.Write(field.Name + ": ");
        // フィールドの値がテキストかどうかを確認し、出力する
        PageTextArea area = field.PageArea as PageTextArea;
        Console.WriteLine(area == null ? "Not a template field" : area.Text);
    }
}
```

### 関連項目

* class [FieldData](../../fielddata)
* class [DocumentData](../../documentdata)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

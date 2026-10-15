---
title: "GetFieldsByName"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "名前が fieldName と等しいフィールド データのコレクションを返します。"
type: docs
weight: 50
url: /ja/net/groupdocs.parser.data/documentdata/getfieldsbyname/
---

## DocumentData.GetFieldsByName method

名前が *fieldName* と等しいフィールドデータのコレクションを返します。

```csharp
public IList<FieldData> GetFieldsByName(string fieldName)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| fieldName | 文字列 | フィールドの名前です。 |

### 戻り値

[`FieldData`](../../fielddata) オブジェクトのコレクションです。フィールド データが見つからない場合は空のコレクションです。

### 例

フィールド名でフィールドを検索:

```csharp
// 名前が "Address" のすべてのフィールドを取得する
IList<FieldData> addressFields = data.GetFieldsByName("Address");
if(addressFields.Count == 0) {
    Console.WriteLine("Address not found");
}
else {
    Console.WriteLine("Address");
    // フィールド コレクションを反復処理する
    for (int i = 0; i < addressFields.Count; i++) {
        PageTextArea area = addressFields[i].PageArea as PageTextArea;
        Console.WriteLine(area == null ? "Not a template field" : area.Text);       
         
        // 関連フィールドの場合:
        if(addressFields[i].LinkedField != null) {
            Console.Write("Linked to ");
            PageTextArea linkedArea = addressFields[i].LinkedField.PageArea as PageTextArea;
            Console.WriteLine(area == null ? "Not a template field" : area.Text);           
        }
    }
}
```

[`FieldData`](../../fielddata) class represents field data. Depending on the field [`PageArea`](../../fielddata/pagearea) property can contain any of the inheritors of [`PageArea`](../../pagearea) class. For example, [`ParseForm`](../../../groupdocs.parser/parser/parseform) method extracts only text fields.

### 関連項目

* class [FieldData](../../fielddata)
* class [DocumentData](../../documentdata)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

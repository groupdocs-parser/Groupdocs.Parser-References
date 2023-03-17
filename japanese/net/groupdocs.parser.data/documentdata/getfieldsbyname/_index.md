---
title: GetFieldsByName
second_title: GroupDocs.Parser for .NET API リファレンス
description: 名前が等しいフィールド データのコレクションを返しますfieldName.
type: docs
weight: 50
url: /ja/net/groupdocs.parser.data/documentdata/getfieldsbyname/
---
## DocumentData.GetFieldsByName method

名前が等しいフィールド データのコレクションを返します*fieldName*.

```csharp
public IList<FieldData> GetFieldsByName(string fieldName)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| fieldName | String | フィールドの名前。 |

### 戻り値

のコレクション[`FieldData`](../../fielddata)オブジェクト;フィールド データが見つからない場合は空のコレクション。

### 例

フィールド名でフィールドを検索:

[`FieldData`](../../fielddata)クラスはフィールドデータを表します。分野にもよりますが[`PageArea`](../../fielddata/pagearea)property には、の継承者のいずれかを含めることができます[`PageArea`](../../pagearea)クラス。例えば、[`ParseForm`](../../../groupdocs.parser/parser/parseform) method は、テキスト フィールドのみを抽出します。

```csharp
// 「住所」という名前のすべてのフィールドを取得します
IList<FieldData> addressFields = data.GetFieldsByName("Address");
if(addressFields.Count == 0) {
    Console.WriteLine("Address not found");
}
else {
    Console.WriteLine("Address");
    // フィールド コレクションを反復処理します
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

### 関連項目

* class [FieldData](../../fielddata)
* class [DocumentData](../../documentdata)
* 名前空間 [GroupDocs.Parser.Data](../../documentdata)
* 組み立て [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
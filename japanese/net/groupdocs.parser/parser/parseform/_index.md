---
title: "ParseForm"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ドキュメントフォームを解析します。"
type: docs
weight: 240
url: /ja/net/groupdocs.parser/parser/parseform/
---

## Parser.ParseForm method

ドキュメントフォームを解析します。

```csharp
public DocumentData ParseForm()
```

### 戻り値

抽出されたデータを含む [`DocumentData`](../../../groupdocs.parser.data/documentdata) クラスのインスタンス; テンプレートによる解析がサポートされていない場合は `null`。

### 備考

**Learn more:**

* [Extract data from PDF forms](https://docs.groupdocs.com/display/parsernet/Extract+data+from+PDF+forms)
* [Working with extracted data](https://docs.groupdocs.com/display/parsernet/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+PDF+documents)

### 例

次の例は、ドキュメントのフォームを解析する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // PDF ドキュメントからデータを抽出する
    DocumentData data = parser.ParseForm();
    // 抽出されたデータを反復処理する
    for (int i = 0; i<data.Count; i++)
    {
        Console.Write(data[i].Name + ": ");
        PageTextArea area = data[i].PageArea as PageTextArea;
        Console.WriteLine(area == null ? "Not a template field" : area.Text);
    }
}
```

### 関連項目

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

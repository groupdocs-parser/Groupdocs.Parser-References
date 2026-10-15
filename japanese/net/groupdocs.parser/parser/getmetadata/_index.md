---
title: "GetMetadata"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ドキュメントからメタデータを抽出します。"
type: docs
weight: 140
url: /ja/net/groupdocs.parser/parser/getmetadata/
---

## Parser.GetMetadata method

ドキュメントからメタデータを抽出します。

```csharp
public IEnumerable<MetadataItem> GetMetadata()
```

### 戻り値

メタデータ項目のコレクションです。メタデータ抽出がサポートされていない場合は `null` になります。

### 備考

**Learn more:**

* [Extract metadata from documents](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+documents)
* [Extract metadata from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+Word+documents)
* [Extract metadata from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+Excel+spreadsheets)
* [Extract metadata from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+PowerPoint+presentations)
* [Extract metadata from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+PDF+documents)
* [Extract metadata from Emails](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Emails)

### 例

次の例は、ドキュメントからメタデータを抽出する方法を示しています。

```csharp
// Parser クラスのインスタンスを作成します
using(Parser parser = new Parser(filePath))
{
    // ドキュメントからメタデータを抽出する
    IEnumerable<MetadataItem> metadata = parser.GetMetadata();
    // メタデータ抽出がサポートされているか確認する
    if(metadata == null)
    {
        Console.WriteLine("Metatada extraction isn't supported");
    }
 
    // メタデータ項目を反復処理する
    foreach(MetadataItem item in metadata)
    {
        // 項目名と値を出力する
        Console.WriteLine(string.Format("{0}: {1}", item.Name, item.Value));
    }
}
```

### 関連項目

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

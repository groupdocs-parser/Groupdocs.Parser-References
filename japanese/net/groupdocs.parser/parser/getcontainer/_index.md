---
title: "GetContainer"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "添付ファイルや ZIP アーカイブなどを含む形式を扱うために、ドキュメントからコンテナオブジェクトを抽出します。"
type: docs
weight: 80
url: /ja/net/groupdocs.parser/parser/getcontainer/
---

## Parser.GetContainer method

添付ファイルやZIPアーカイブなどを含む形式を扱うために、ドキュメントからコンテナオブジェクトを抽出します。

```csharp
public IEnumerable<ContainerItem> GetContainer()
```

### 戻り値

コンテナ項目のコレクション; コンテナ抽出がサポートされていない場合は `null`。

### 備考

形式が添付ファイルの抽出をサポートしているか確認するには、[Supported Document Formats](https://docs.groupdocs.com/parser/net/supported-document-formats/) (**Extract Containers and Attachments** 列) を参照してください。

**Learn more:**

* [Extract data from attachments and ZIP archives](https://docs.groupdocs.com/display/parsernet/Extract+data+from+attachments+and+ZIP+archives)
* [Iterate through container items](https://docs.groupdocs.com/display/parsernet/Iterate+through+container+items)
* [Extract attachments from PDF portfolios](https://docs.groupdocs.com/display/parsernet/Extract+attachments+from+PDF+portfolios)
* [Extract attachments from Emails](https://docs.groupdocs.com/display/parsernet/Extract+attachments+from+Emails)
* [Extract emails from Outlook Storage](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+Outlook+Storage)
* [Extract text from ZIP archive files](https://docs.groupdocs.com/display/parsernet/Extract+text+from+ZIP+archive+files)

### 例

次の例は、コンテナから添付ファイルを抽出する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using(Parser parser = new Parser(filePath))
{
    // コンテナから添付ファイルを抽出する
    IEnumerable<ContainerItem> attachments = parser.GetContainer();
    // コンテナ抽出がサポートされているか確認する
    if(attachments == null)
    {
        Console.WriteLine("Container extraction isn't supported");
    }
 
    // 添付ファイルを反復処理する
    foreach(ContainerItem item in attachments)
    {
        // 項目名とサイズを印刷する
        Console.WriteLine(string.Format("{0}: {1}", item.Name, item.Size));
    }
}
```

### 関連項目

* class [ContainerItem](../../../groupdocs.parser.data/containeritem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

---
title: "GetDocumentInfo"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ドキュメントに関する一般情報を返します。"
type: docs
weight: 90
url: /ja/net/groupdocs.parser/parser/getdocumentinfo/
---

## Parser.GetDocumentInfo method

ドキュメントに関する一般情報を返します。

```csharp
public IDocumentInfo GetDocumentInfo()
```

### 戻り値

[`IDocumentInfo`](../../../groupdocs.parser.options/idocumentinfo) インターフェイスを実装するクラスのインスタンスです。

### 備考

**Learn more:**

* [Get document info](https://docs.groupdocs.com/display/parsernet/Get+document+info)
* [Detect encoding](https://docs.groupdocs.com/display/parsernet/Detect+encoding)

### 例

次の例は、ドキュメント情報を取得する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using(Parser parser = new Parser(filePath))
{
    // ドキュメント情報を取得する
    IDocumentInfo info = parser.GetDocumentInfo();

    Console.WriteLine(string.Format("FileType: {0}", info.FileType));
    Console.WriteLine(string.Format("PageCount: {0}", info.PageCount));
    Console.WriteLine(string.Format("Size: {0}", info.Size));
}
```

### 関連項目

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

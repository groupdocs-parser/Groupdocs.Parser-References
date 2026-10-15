---
title: "機能"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "サポートされている機能を取得します。"
type: docs
weight: 20
url: /ja/net/groupdocs.parser/parser/features/
---

## Parser.Features property

サポートされている機能を取得します。

```csharp
public Features Features { get; }
```

### Property Value

サポートされている機能を表す [`Features`](../../../groupdocs.parser.options/features) クラスのインスタンスです。

### 備考

**Learn more:**

* [Get supported features](https://docs.groupdocs.com/display/parsernet/Get+supported+features)

### 例

機能がサポートされていない場合、メソッドは値の代わりに `null` を返します。いくつかの操作はかなりの時間がかかる可能性があります。そのため、機能のサポートを確認するだけでメソッドを呼び出すのは最適ではありません。この目的のために Features プロパティが使用されます:

```csharp
using(Parser parser = new Parser("doc.zip"))
{
    if(!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported");
        return;
    }
 
    using(TextReader reader = parser.GetText())
    {
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

### 関連項目

* class [Features](../../../groupdocs.parser.options/features)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

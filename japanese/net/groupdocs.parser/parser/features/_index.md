---
title: Features
second_title: GroupDocs.Parser for .NET API リファレンス
description: サポートされている機能を取得します
type: docs
weight: 20
url: /ja/net/groupdocs.parser/parser/features/
---
## Parser.Features property

サポートされている機能を取得します。

```csharp
public Features Features { get; }
```

### プロパティ値

のインスタンス[`Features`](../../../groupdocs.parser.options/features)サポートされている機能を表すクラス。

### 備考

**もっと詳しく知る：**

* [サポートされている機能を入手する](https://docs.groupdocs.com/display/parsernet/Get+supported+features)

### 例

機能がサポートされていない場合、メソッドは戻ります`ヌル`値の代わりに。 一部の操作にはかなりの時間がかかる場合があります。そのため、機能のサポートを確認するためだけにメソッドを呼び出すのは最適ではありません。 この目的のために Features プロパティが使用されます:

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
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

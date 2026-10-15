---
title: "GetConsumptionQuantity"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "処理された MB の量を取得します。"
type: docs
weight: 40
url: /ja/net/groupdocs.parser/metered/getconsumptionquantity/
---

## Metered.GetConsumptionQuantity method

処理された MB の量を取得します。

```csharp
public static decimal GetConsumptionQuantity()
```

### 戻り値

消費量を表す十進数値です。

### 例

以下の例は、処理された MB の量を取得する方法を示しています。

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);

decimal mbProcessed = Metered.GetConsumptionQuantity();
```

### 関連項目

* class [Metered](../../metered)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

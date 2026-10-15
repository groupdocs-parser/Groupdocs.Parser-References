---
title: "GetConsumptionCredit"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "消費されたクレジットの数を取得します。"
type: docs
weight: 30
url: /ja/net/groupdocs.parser/metered/getconsumptioncredit/
---

## Metered.GetConsumptionCredit method

消費されたクレジットの数を取得します。

```csharp
public static decimal GetConsumptionCredit()
```

### 戻り値

消費クレジットを表す十進数値です。

### 例

以下の例は、消費されたクレジット数を取得する方法を示しています。

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);

decimal creditsConsumed = Metered.GetConsumptionCredit();
```

### 関連項目

* class [Metered](../../metered)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

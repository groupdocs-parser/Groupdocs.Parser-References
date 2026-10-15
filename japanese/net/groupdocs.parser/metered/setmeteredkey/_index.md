---
title: "SetMeteredKey"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "Metered キーで製品を有効化します。"
type: docs
weight: 20
url: /ja/net/groupdocs.parser/metered/setmeteredkey/
---

## Metered.SetMeteredKey method

Metered キーで製品を有効化します。

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| publicKey | 文字列 | 公開鍵です。 |
| privateKey | 文字列 | プライベートキー |

### 例

以下の例は、Metered キーを使用して製品をアクティブ化する方法を示しています。

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);
```

### 関連項目

* class [Metered](../../metered)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->

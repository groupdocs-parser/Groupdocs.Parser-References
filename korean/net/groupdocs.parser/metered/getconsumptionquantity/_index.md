---
title: GetConsumptionQuantity
second_title: .NET API 참조용 GroupDocs.Parser
description: 처리된 MB 양을 검색합니다.
type: docs
weight: 40
url: /ko/net/groupdocs.parser/metered/getconsumptionquantity/
---
## Metered.GetConsumptionQuantity method

처리된 MB 양을 검색합니다.

```csharp
public static decimal GetConsumptionQuantity()
```

### 반환 값

소비 수량을 나타내는 10진수 값입니다.

### 예

다음 예제는 처리된 MB 양을 검색하는 방법을 보여줍니다.

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);

decimal mbProcessed = Metered.GetConsumptionQuantity();
```

### 또한보십시오

* class [Metered](../../metered)
* 네임스페이스 [GroupDocs.Parser](../../metered)
* 집회 [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

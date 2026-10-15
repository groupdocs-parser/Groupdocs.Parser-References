---
title: "GetConsumptionCredit"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Получает количество использованных кредитов."
type: docs
weight: 30
url: /ru/net/groupdocs.parser/metered/getconsumptioncredit/
---

## Metered.GetConsumptionCredit method

Получает количество использованных кредитов.

```csharp
public static decimal GetConsumptionCredit()
```

### Возвращаемое значение

Десятичное значение, представляющее кредит потребления.

### Примеры

Следующий пример демонстрирует, как получить количество использованных кредитов.

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);

decimal creditsConsumed = Metered.GetConsumptionCredit();
```

### См. также

* class [Metered](../../metered)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->

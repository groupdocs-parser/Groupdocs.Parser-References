---
title: "GetConsumptionQuantity"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Получает объём обработанных мегабайт."
type: docs
weight: 40
url: /ru/net/groupdocs.parser/metered/getconsumptionquantity/
---

## Metered.GetConsumptionQuantity method

Получает объём обработанных мегабайт.

```csharp
public static decimal GetConsumptionQuantity()
```

### Возвращаемое значение

Десятичное значение, представляющее количество потребления.

### Примеры

Следующий пример демонстрирует, как получить количество обработанных МБ.

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);

decimal mbProcessed = Metered.GetConsumptionQuantity();
```

### См. также

* class [Metered](../../metered)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->

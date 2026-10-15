---
title: "GetConsumptionQuantity"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Liest die Menge der verarbeiteten MB."
type: docs
weight: 40
url: /de/net/groupdocs.parser/metered/getconsumptionquantity/
---

## Metered.GetConsumptionQuantity method

Liest die Menge der verarbeiteten MB.

```csharp
public static decimal GetConsumptionQuantity()
```

### Rückgabewert

Ein Dezimalwert, der die Verbrauchsmenge darstellt.

### Beispiele

Das folgende Beispiel zeigt, wie die Menge an verarbeiteten MBs abgerufen wird.

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);

decimal mbProcessed = Metered.GetConsumptionQuantity();
```

### Siehe auch

* class [Metered](../../metered)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->

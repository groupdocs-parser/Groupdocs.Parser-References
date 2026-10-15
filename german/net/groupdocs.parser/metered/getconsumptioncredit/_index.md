---
title: "GetConsumptionCredit"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Liest die Anzahl der verbrauchten Credits."
type: docs
weight: 30
url: /de/net/groupdocs.parser/metered/getconsumptioncredit/
---

## Metered.GetConsumptionCredit method

Liest die Anzahl der verbrauchten Credits.

```csharp
public static decimal GetConsumptionCredit()
```

### Rückgabewert

Ein Dezimalwert, der das Verbrauchsguthaben darstellt.

### Beispiele

Das folgende Beispiel zeigt, wie die Anzahl der verbrauchten Guthaben abgerufen wird.

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);

decimal creditsConsumed = Metered.GetConsumptionCredit();
```

### Siehe auch

* class [Metered](../../metered)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->

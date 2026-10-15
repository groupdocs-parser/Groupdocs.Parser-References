---
title: "SetMeteredKey"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Aktiviert das Produkt mit Metered-Schlüsseln."
type: docs
weight: 20
url: /de/net/groupdocs.parser/metered/setmeteredkey/
---

## Metered.SetMeteredKey method

Aktiviert das Produkt mit Metered-Schlüsseln.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| publicKey | String | Ein öffentlicher Schlüssel. |
| privateKey | String | Ein privater Schlüssel |

### Beispiele

Das folgende Beispiel zeigt, wie man ein Produkt mit Metered-Schlüsseln aktiviert.

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);
```

### Siehe auch

* class [Metered](../../metered)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->

---
title: SetMeteredKey
second_title: GroupDocs.Parser för .NET API-referens
description: Aktiverar produkt med uppmätta nycklar.
type: docs
weight: 20
url: /sv/net/groupdocs.parser/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Aktiverar produkt med uppmätta nycklar.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| publicKey | String | En offentlig nyckel. |
| privateKey | String | En privat nyckel |

### Exempel

Följande exempel visar hur man aktiverar produkten med mätbara nycklar.

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);
```

### Se även

* class [Metered](../../metered)
* namnutrymme [GroupDocs.Parser](../../metered)
* hopsättning [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
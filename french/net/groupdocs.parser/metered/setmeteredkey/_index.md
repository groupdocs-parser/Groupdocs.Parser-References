---
title: "SetMeteredKey"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Active le produit avec des clés Metered."
type: docs
weight: 20
url: /fr/net/groupdocs.parser/metered/setmeteredkey/
---

## Metered.SetMeteredKey method

Active le produit avec des clés Metered.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| publicKey | Chaîne | Une clé publique. |
| privateKey | Chaîne | Une clé privée |

### Exemples

L'exemple suivant montre comment activer le produit avec des clés mesurées.

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);
```

### Voir aussi

* class [Metered](../../metered)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->

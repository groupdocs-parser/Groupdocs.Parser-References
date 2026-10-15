---
title: "TryParse"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Convertit la représentation sous forme de chaîne d'un point en son équivalent de classe. Une valeur de retour indique si la conversion a réussi ou échoué."
type: docs
weight: 80
url: /fr/net/groupdocs.parser.data/point/tryparse/
---

## Point.TryParse method

Convertit la représentation sous forme de chaîne d'un point en son équivalent de classe. Une valeur de retour indique si la conversion a réussi ou échoué.

```csharp
public static bool TryParse(string s, out Point point)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| s | Chaîne | Une chaîne contenant un point à convertir. |
| point | Point& | Lorsque la méthode retourne, elle contient l'instance de la classe [`Point`](../../point) équivalente à la valeur spécifiée dans le paramètre *s*, si la conversion a réussi ; sinon, `null`. |

### Valeur de retour

`true` si *s* est converti avec succès ; sinon, `false`.

### Voir aussi

* class [Point](../../point)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->

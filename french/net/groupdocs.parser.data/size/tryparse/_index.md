---
title: "TryParse"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Convertit la représentation sous forme de chaîne d'une taille en son équivalent de classe. Une valeur de retour indique si la conversion a réussi ou échoué."
type: docs
weight: 70
url: /fr/net/groupdocs.parser.data/size/tryparse/
---

## Size.TryParse method

Convertit la représentation sous forme de chaîne d'une taille en son équivalent de classe. Une valeur de retour indique si la conversion a réussi ou échoué.

```csharp
public static bool TryParse(string s, out Size size)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| s | Chaîne | Une chaîne contenant une taille à convertir. |
| size | Size& | Lorsque la méthode retourne, elle contient l'instance de la classe [`Size`](../../size) équivalente à la valeur spécifiée dans le paramètre *s*, si la conversion a réussi ; sinon, `null`. |

### Valeur de retour

`true` si *s* est converti avec succès ; sinon, `false`.

### Voir aussi

* class [Size](../../size)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->

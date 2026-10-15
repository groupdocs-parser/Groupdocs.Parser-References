---
title: "PageArea"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Obtient la valeur du champ."
type: docs
weight: 30
url: /fr/net/groupdocs.parser.data/fielddata/pagearea/
---

## FieldData.PageArea property

Obtient la valeur du champ.

```csharp
public PageArea PageArea { get; }
```

### Property Value

Une instance de la classe [`PageArea`](../../pagearea) qui représente la valeur du champ.

### Exemples

Selon le champ, la propriété `PageArea` peut contenir n'importe lequel des héritiers de la classe [`PageArea`](../../pagearea). Par exemple, la méthode [`ParseForm`](../../../groupdocs.parser/parser/parseform) extrait uniquement les champs texte.

```csharp
// Obtenir les données du champ
FieldData field = data[i];
// Vérifier si les données du champ contiennent un texte
if(field.PageArea is PageTextArea)
{
    // Imprimer la valeur du texte du champ
    Console.WriteLine(field.Text);
}
```

### Voir aussi

* class [PageArea](../../pagearea)
* class [FieldData](../../fielddata)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->

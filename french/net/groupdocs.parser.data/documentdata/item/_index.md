---
title: "Élément"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Obtient les données de champ par indice."
type: docs
weight: 20
url: /fr/net/groupdocs.parser.data/documentdata/item/
---

## DocumentData indexer

Obtient les données de champ par indice.

```csharp
public FieldData this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'index basé sur zéro du champ. |

### Valeur de retour

Une instance de la classe [`FieldData`](../../fielddata).

### Exemples

Itération via tous les champs :

```csharp
for (int i = 0; i < data.Count; i++)
{
    Console.Write(data[i].Name + ": ");
    PageTextArea area = data[i].PageArea as PageTextArea;
    Console.WriteLine(area == null ? "Not a template field" : area.Text);
}
```

[`FieldData`](../../fielddata) class represents field data. Depending on the field [`PageArea`](../../fielddata/pagearea) property can contain any of the inheritors of [`PageArea`](../../pagearea) class. For example, [`ParseForm`](../../../groupdocs.parser/parser/parseform) method extracts only text fields:

```csharp
// Créer l'analyseur
using (Parser parser = new Parser(filePath))
{
    // Extraire les données du formulaire PDF
    DocumentData data = parser.ParseForm();
    // Itérer sur les champs extraits
    for (int i = 0; i < data.Count; i++)
    {
        // Obtenir le champ extrait
        FieldData field = data[i];
        // Afficher le nom du champ
        Console.Write(field.Name + ": ");
        // Vérifier si la valeur du champ est un texte et l'afficher
        PageTextArea area = field.PageArea as PageTextArea;
        Console.WriteLine(area == null ? "Not a template field" : area.Text);
    }
}
```

### Voir aussi

* class [FieldData](../../fielddata)
* class [DocumentData](../../documentdata)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->

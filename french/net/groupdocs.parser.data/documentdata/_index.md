---
title: "DocumentData"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Représente les données du document. Il se compose d'objets FieldData./fielddata qui contiennent les données de champ du document."
type: docs
weight: 730
url: /fr/net/groupdocs.parser.data/documentdata/
---

## DocumentData class

Représente les données du document. Il se compose d'objets [`FieldData`](../fielddata) qui contiennent les données de champ du document.

```csharp
public class DocumentData : IEnumerable<FieldData>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../groupdocs.parser.data/documentdata/count) { get; } | Obtient le nombre total des données de champs. |
| [Item](../../groupdocs.parser.data/documentdata/item) { get; } | Obtient les données de champ par indice. |
| [Template](../../groupdocs.parser.data/documentdata/template) { get; } | Obtient le modèle. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetEnumerator](../../groupdocs.parser.data/documentdata/getenumerator)() | Renvoie un énumérateur pour les données de champs. |
| [GetFieldsByName](../../groupdocs.parser.data/documentdata/getfieldsbyname)(string) | Renvoie la collection de données de champ dont le nom est égal à *fieldName*. |

### Remarques

Une instance de la classe [`DocumentData`](../documentdata) est utilisée comme valeur de retour des méthodes [`ParseByTemplate`](../../groupdocs.parser/parser/parsebytemplate) et [`ParseForm`](../../groupdocs.parser/parser/parseform). Voir les exemples d'utilisation là-bas.

### Voir aussi

* class [FieldData](../fielddata)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->

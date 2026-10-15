---
title: "DocumentPageData"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Représente les données de la page du document. Il se compose d'objets FieldData./fielddata qui contiennent les données de champ de la page du document."
type: docs
weight: 740
url: /fr/net/groupdocs.parser.data/documentpagedata/
---

## DocumentPageData class

Représente les données de la page du document. Il se compose d'objets [`FieldData`](../fielddata) qui contiennent les données de champ de la page du document.

```csharp
public sealed class DocumentPageData : DocumentData
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../groupdocs.parser.data/documentdata/count) { get; } | Obtient le nombre total des données de champs. |
| [Item](../../groupdocs.parser.data/documentdata/item) { get; } | Obtient les données de champ par indice. |
| [PageIndex](../../groupdocs.parser.data/documentpagedata/pageindex) { get; } | Obtient l'index de la page. |
| [Template](../../groupdocs.parser.data/documentdata/template) { get; } | Obtient le modèle. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetEnumerator](../../groupdocs.parser.data/documentdata/getenumerator)() | Renvoie un énumérateur pour les données de champs. |
| [GetFieldsByName](../../groupdocs.parser.data/documentdata/getfieldsbyname)(string) | Renvoie la collection de données de champ dont le nom est égal à *fieldName*. |

### Voir aussi

* class [DocumentData](../documentdata)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->

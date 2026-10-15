---
title: "TocItem"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Représente l'élément utilisé dans la fonctionnalité d'extraction de la table des matières."
type: docs
weight: 920
url: /fr/net/groupdocs.parser.data/tocitem/
---

## TocItem class

Représente l'élément utilisé dans la fonctionnalité d'extraction de la table des matières.

```csharp
public class TocItem
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [TocItem](tocitem)(int, string, int?) | Initialise une nouvelle instance de la classe [`TocItem`](../tocitem). |

## Propriétés

| Nom | Description |
| --- | --- |
| [Depth](../../groupdocs.parser.data/tocitem/depth) { get; } | Obtient le niveau de profondeur. |
| [PageIndex](../../groupdocs.parser.data/tocitem/pageindex) { get; } | Obtient l'index de la page. |
| [Text](../../groupdocs.parser.data/tocitem/text) { get; } | Obtient le texte. |

## Méthodes

| Nom | Description |
| --- | --- |
| virtual [ExtractText](../../groupdocs.parser.data/tocitem/extracttext)() | Extrait un texte du document auquel l'objet [`TocItem`](../tocitem) fait référence. |

### Remarques

Une instance de la classe [`TocItem`](../tocitem) est utilisée comme valeur de retour des méthodes [`GetToc`](../../groupdocs.parser/parser/gettoc). Voir les exemples d'utilisation là-bas.

### Voir aussi

* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->

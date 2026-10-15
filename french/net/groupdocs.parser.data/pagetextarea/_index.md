---
title: "PageTextArea"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Représente une zone de texte de page utilisée pour représenter une valeur de texte dans la fonctionnalité d'analyse par modèle ou d'analyse de formulaire."
type: docs
weight: 860
url: /fr/net/groupdocs.parser.data/pagetextarea/
---

## PageTextArea class

Représente une zone de texte de page utilisée pour représenter une valeur de texte dans la fonctionnalité d'analyse par modèle ou d'analyse de formulaire.

```csharp
public sealed class PageTextArea : PageArea
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PageTextArea](pagetextarea#constructor)(IEnumerable&lt;PageTextArea&gt;, Page) | Initialise une nouvelle instance de la classe [`PageTextArea`](../pagetextarea). |
| [PageTextArea](pagetextarea#constructor_1)(string, Page, Rectangle) | Initialise une nouvelle instance de la classe [`PageTextArea`](../pagetextarea). |
| [PageTextArea](pagetextarea#constructor_2)(string, double?, TextStyle, Page, Rectangle) | Initialise une nouvelle instance de la classe [`PageTextArea`](../pagetextarea). |

## Propriétés

| Nom | Description |
| --- | --- |
| [Areas](../../groupdocs.parser.data/pagetextarea/areas) { get; } | Obtient la collection des zones de texte enfants de la page. |
| [BaseLine](../../groupdocs.parser.data/pagetextarea/baseline) { get; } | Obtient la ligne de base. |
| [Page](../../groupdocs.parser.data/pagearea/page) { get; } | Obtient les informations de la page du document telles que l'index de page et la taille de page. |
| [Rectangle](../../groupdocs.parser.data/pagearea/rectangle) { get; } | Obtient la zone rectangulaire. |
| [Text](../../groupdocs.parser.data/pagetextarea/text) { get; } | Obtient le texte. |
| [TextStyle](../../groupdocs.parser.data/pagetextarea/textstyle) { get; } | Obtient le style de texte tel que la taille de police, le nom de police, etc. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [ToString](../../groupdocs.parser.data/pagetextarea/tostring)() | Convertit la valeur de cette instance en String. |

### Remarques

Une instance de la classe [`PageTextArea`](../pagetextarea) est utilisée comme valeur de retour des méthodes suivantes :

* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)
* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)
* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)
* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)

Une instance de la classe [`PageTextArea`](../pagetextarea) est également utilisée comme valeur de la propriété [`PageArea`](../fielddata/pagearea).

Voir les exemples d'utilisation là-bas.

La zone de texte peut être simple ou composite. Dans le premier cas, elle contient un texte délimité par une zone rectangulaire. Dans le second cas, elle contient d'autres zones de texte ; les propriétés du texte et du tableau sont calculées à partir des zones de texte enfants.

### Voir aussi

* class [PageArea](../pagearea)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->

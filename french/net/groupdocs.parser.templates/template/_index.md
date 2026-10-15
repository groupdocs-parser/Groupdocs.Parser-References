---
title: "Modèle"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Fournit le modèle de page du document. Il se compose d'objets TemplateItem./templateitem qui représentent les éléments du modèle tels que les champs de texte et les définitions de tableau."
type: docs
weight: 50
url: /fr/net/groupdocs.parser.templates/template/
---

## Template class

Fournit le modèle de page du document. Il se compose d'objets [`TemplateItem`](../templateitem) qui représentent les éléments du modèle tels que les champs de texte et les définitions de tableau.

```csharp
public sealed class Template : IEnumerable<TemplateItem>
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Template](template#constructor)(IEnumerable&lt;TemplateItem&gt;) | Initialise une nouvelle instance de la classe [`Template`](../template). |
| [Template](template#constructor_1)(IEnumerable&lt;TemplateItem&gt;, TemplateOptions) | Initialise une nouvelle instance de la classe [`Template`](../template) avec des options de modèle. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../groupdocs.parser.templates/template/count) { get; } | Obtient le nombre total d'éléments du modèle. |
| [IsOcrCompatible](../../groupdocs.parser.templates/template/isocrcompatible) { get; } | Obtient la valeur qui indique si le modèle est compatible avec l'OCR. |
| [Item](../../groupdocs.parser.templates/template/item) { get; } | Obtient l'élément du modèle par un indice. |
| [Options](../../groupdocs.parser.templates/template/options) { get; } | Obtient les options du modèle. |

## Méthodes

| Nom | Description |
| --- | --- |
| static [Load](../../groupdocs.parser.templates/template/load#load)(Stream) | Charge un modèle depuis un flux. |
| static [Load](../../groupdocs.parser.templates/template/load#load_1)(string) | Charge un modèle depuis un fichier. |
| [GetEnumerator](../../groupdocs.parser.templates/template/getenumerator)() | Renvoie un énumérateur pour les éléments du modèle. |
| [Save](../../groupdocs.parser.templates/template/save#save)(Stream) | Enregistre un modèle dans un flux. |
| [Save](../../groupdocs.parser.templates/template/save#save_1)(string) | Enregistre un modèle dans un fichier. |

### Remarques

**Learn more:**

* [Working with templates](https://docs.groupdocs.com/display/parsernet/Working+with+templates)

### Voir aussi

* class [TemplateItem](../templateitem)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->

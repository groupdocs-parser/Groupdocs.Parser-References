---
title: "TemplateField"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Fournit le champ de texte du modèle."
type: docs
weight: 80
url: /fr/net/groupdocs.parser.templates/templatefield/
---

## TemplateField class

Fournit le champ de texte du modèle.

```csharp
public sealed class TemplateField : TemplateItem
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [TemplateField](templatefield#constructor)(TemplatePosition, string) | Initialise une nouvelle instance de la classe [`TemplateField`](../templatefield). |
| [TemplateField](templatefield#constructor_1)(TemplatePosition, string, double?) | Initialise une nouvelle instance de la classe [`TemplateField`](../templatefield). |
| [TemplateField](templatefield#constructor_2)(TemplatePosition, string, double?, bool) | Initialise une nouvelle instance de la classe [`TemplateField`](../templatefield). |

## Propriétés

| Nom | Description |
| --- | --- |
| [IsHidden](../../groupdocs.parser.templates/templatefield/ishidden) { get; set; } | Obtient ou définit le drapeau du champ de modèle caché. |
| [Name](../../groupdocs.parser.templates/templateitem/name) { get; } | Obtient le nom de l'élément de modèle. |
| [PageWidth](../../groupdocs.parser.templates/templateitem/pagewidth) { get; } | Obtient la largeur de la page qui a été utilisée pour créer l'élément de modèle. |
| [Position](../../groupdocs.parser.templates/templatefield/position) { get; } | Obtient la valeur qui décrit comment trouver le champ de modèle sur la page du document. |
| [UseUpperCaseName](../../groupdocs.parser.templates/templateitem/useuppercasename) { get; } | Obtient une valeur booléenne qui indique si un `Name` a été converti en MAJUSCULES. |
| [Value](../../groupdocs.parser.templates/templatefield/value) { get; set; } | Obtient ou définit la valeur du champ de modèle. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Scale](../../groupdocs.parser.templates/templatefield/scale)(double) | Redimensionne cet élément de modèle par un facteur donné. |

### Remarques

Les champs de texte sont définis par leur position sur la page. Il existe trois manières de définir un champ de texte :

* [`Using the rectangular area`](../templatefixedposition)
* [`Using the regular expression`](../templateregexposition)
* [`Using the linked field`](../templatelinkedposition)

### Voir aussi

* class [TemplateItem](../templateitem)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->

---
title: "TemplateTable"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Fournit le tableau du modèle."
type: docs
weight: 160
url: /fr/net/groupdocs.parser.templates/templatetable/
---

## TemplateTable class

Fournit le tableau du modèle.

```csharp
public sealed class TemplateTable : TemplateItem
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [TemplateTable](templatetable#constructor)(TemplateTableLayout, string) | Initialise une nouvelle instance de la classe [`TemplateTable`](../templatetable) avec le nom EN MAJUSCULE. |
| [TemplateTable](templatetable#constructor_3)(TemplateTableParameters, string) | Initialise une nouvelle instance de la classe [`TemplateTable`](../templatetable). |
| [TemplateTable](templatetable#constructor_1)(TemplateTableLayout, string, double?) | Initialise une nouvelle instance de la classe [`TemplateTable`](../templatetable) avec le nom EN MAJUSCULE. |
| [TemplateTable](templatetable#constructor_4)(TemplateTableParameters, string, double?) | Initialise une nouvelle instance de la classe [`TemplateTable`](../templatetable). |
| [TemplateTable](templatetable#constructor_2)(TemplateTableLayout, string, double?, bool) | Initialise une nouvelle instance de la classe [`TemplateTable`](../templatetable). |
| [TemplateTable](templatetable#constructor_5)(TemplateTableParameters, string, double?, bool) | Initialise une nouvelle instance de la classe [`TemplateTable`](../templatetable). |

## Propriétés

| Nom | Description |
| --- | --- |
| [Layout](../../groupdocs.parser.templates/templatetable/layout) { get; } | Obtient la mise en page du tableau. |
| [Name](../../groupdocs.parser.templates/templateitem/name) { get; } | Obtient le nom de l'élément de modèle. |
| [PageWidth](../../groupdocs.parser.templates/templateitem/pagewidth) { get; } | Obtient la largeur de la page qui a été utilisée pour créer l'élément de modèle. |
| [Parameters](../../groupdocs.parser.templates/templatetable/parameters) { get; } | Obtient les paramètres pour détecter le tableau en mode automatique. |
| [UseUpperCaseName](../../groupdocs.parser.templates/templateitem/useuppercasename) { get; } | Obtient une valeur booléenne qui indique si un `Name` a été converti en MAJUSCULES. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Scale](../../groupdocs.parser.templates/templatetable/scale)(double) | Redimensionne cet élément de modèle par un facteur donné. |

### Remarques

Il existe deux manières de définir un tableau:

* Using [`TemplateTableLayout`](../templatetablelayout) class. In this case the table is defined by its position on the page: rectangular area, columns and rows separators.
* Using [`TemplateTableParameters`](../templatetableparameters) class. In this case the table is detected automatically by algorithms with set parameters. See [`TemplateTableParameters`](../templatetableparameters) class for more information.

### Voir aussi

* class [TemplateItem](../templateitem)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->

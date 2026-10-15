---
title: "TemplateFixedPosition"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Fournit une position de champ de modèle définie par la zone rectangulaire."
type: docs
weight: 90
url: /fr/net/groupdocs.parser.templates/templatefixedposition/
---

## TemplateFixedPosition class

Fournit une position de champ de modèle définie par la zone rectangulaire.

```csharp
public sealed class TemplateFixedPosition : TemplatePosition
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [TemplateFixedPosition](templatefixedposition)(Rectangle) | Initialise une nouvelle instance de la classe [`TemplateFixedPosition`](../templatefixedposition). |

## Propriétés

| Nom | Description |
| --- | --- |
| [Rectangle](../../groupdocs.parser.templates/templatefixedposition/rectangle) { get; } | Obtient la zone rectangulaire qui contient le champ de modèle. |

### Exemples

C'est la façon la plus simple de définir la position du champ. Elle nécessite de définir une zone rectangulaire sur la page qui encadre la valeur du champ. Tout le texte contenu (même partiellement) dans la zone rectangulaire sera extrait comme valeur:

```csharp
// Créez un champ de modèle fixe nommé "Address" délimité par un rectangle à la position (35, 160) et de taille (110, 20)
TemplateField templateField = new TemplateField(
    new TemplateFixedPosition(new Rectangle(new Point(35, 160), new Size(110, 20))),
    "Address");
```

### Voir aussi

* class [TemplatePosition](../templateposition)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->

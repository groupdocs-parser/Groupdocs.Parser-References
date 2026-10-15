---
title: "TemplateRegexPosition"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Fournit une position de champ de modèle qui utilise l'expression régulière."
type: docs
weight: 150
url: /fr/net/groupdocs.parser.templates/templateregexposition/
---

## TemplateRegexPosition class

Fournit une position de champ de modèle qui utilise l'expression régulière.

```csharp
public sealed class TemplateRegexPosition : TemplatePosition
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [TemplateRegexPosition](templateregexposition#constructor)(string) | Initialise une nouvelle instance de la classe [`TemplateRegexPosition`](../templateregexposition). |
| [TemplateRegexPosition](templateregexposition#constructor_1)(string, bool) | Initialise une nouvelle instance de la classe [`TemplateRegexPosition`](../templateregexposition). |

## Propriétés

| Nom | Description |
| --- | --- |
| [Expression](../../groupdocs.parser.templates/templateregexposition/expression) { get; } | Obtient l'expression régulière. |
| [MatchCase](../../groupdocs.parser.templates/templateregexposition/matchcase) { get; } | Obtient la valeur indiquant si la casse du texte n'est pas ignorée. |

### Exemples

L'exemple suivant montre la situation où le document contient "Invoice Number INV-12345" puis le champ de modèle peut être défini de la manière suivante :

```csharp
// Créer un champ de modèle regex avec le nom "InvoiceNumber"
TemplateField templateField = new TemplateField(
    new TemplateRegexPosition("Invoice Number\\s+[A-Z0-9\\-]+"),
    "InvoiceNumber");
```

Dans ce cas, la chaîne entière est extraite comme valeur. Pour extraire uniquement une partie de la chaîne, le groupe d'expression régulière "value" est utilisé :

```csharp
// Créer un champ de modèle regex avec le nom "InvoiceNumber" et le groupe "value"
TemplateField templateField = new TemplateField(
    new TemplateRegexPosition("Invoice Number\\s+(?<value>[A-Z0-9\\-]+)"),
    "InvoiceNumber");
```

Dans ce cas, la chaîne "INV-3337" est extraite comme valeur.

### Voir aussi

* class [TemplatePosition](../templateposition)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->

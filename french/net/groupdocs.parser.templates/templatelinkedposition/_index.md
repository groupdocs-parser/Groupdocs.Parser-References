---
title: "TemplateLinkedPosition"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Fournit une position de champ de modèle qui utilise le champ lié."
type: docs
weight: 110
url: /fr/net/groupdocs.parser.templates/templatelinkedposition/
---

## TemplateLinkedPosition class

Fournit une position de champ de modèle qui utilise le champ lié.

```csharp
public sealed class TemplateLinkedPosition : TemplatePosition
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [TemplateLinkedPosition](templatelinkedposition#constructor)(string, Size, TemplateLinkedPositionEdges) | Initialise une nouvelle instance de la classe [`TemplateLinkedPosition`](../templatelinkedposition). |
| [TemplateLinkedPosition](templatelinkedposition#constructor_1)(string, Size, TemplateLinkedPositionEdges, bool) | Initialise une nouvelle instance de la classe [`TemplateLinkedPosition`](../templatelinkedposition) avec le nom du champ lié EN MAJUSCULE. |
| [TemplateLinkedPosition](templatelinkedposition#constructor_2)(string, Size, TemplateLinkedPositionEdges, bool, bool) | Initialise une nouvelle instance de la classe [`TemplateLinkedPosition`](../templatelinkedposition). |

## Propriétés

| Nom | Description |
| --- | --- |
| [AutoScale](../../groupdocs.parser.templates/templatelinkedposition/autoscale) { get; } | Obtient la valeur qui indique si [`SearchArea`](./searcharea) est mise à l'échelle par la taille du champ lié. |
| [Edges](../../groupdocs.parser.templates/templatelinkedposition/edges) { get; } | Obtient les bords du champ lié où un champ est recherché. |
| [LinkedFieldName](../../groupdocs.parser.templates/templatelinkedposition/linkedfieldname) { get; } | Obtient le nom du champ lié. |
| [SearchArea](../../groupdocs.parser.templates/templatelinkedposition/searcharea) { get; } | Obtient la taille de la zone où un champ est recherché. |

### Exemples

L'exemple suivant montre le code pour la situation où il est connu que le champ contenant le numéro de facture est placé à droite de la chaîne "Invoice number" ; le code suivant est utilisé:

```csharp
// Créez un champ de modèle regex pour trouver le texte "Invoice Number"
TemplateField invoice = new TemplateField(new TemplateRegexPosition("Invoice Number"), "Invoice");

// Créez un champ de modèle associé au champ "Invoice" et extrayez la valeur située à sa droite
TemplateField invoiceNumber = new TemplateField(
    new TemplateLinkedPosition("invoice", new Size(100, 15), new TemplateLinkedPositionEdges(false, false, true, false)),
    "InvoiceNumber");
```

### Voir aussi

* class [TemplatePosition](../templateposition)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->

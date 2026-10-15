---
title: "NombrePagesBrutes"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Obtient le nombre total de pages brutes du document."
type: docs
weight: 40
url: /fr/net/groupdocs.parser.options/idocumentinfo/rawpagecount/
---

## IDocumentInfo.RawPageCount property

Obtient le nombre total de pages brutes du document.

```csharp
public int RawPageCount { get; }
```

### Property Value

Une valeur entière qui représente le nombre total de pages brutes.

### Remarques

Utilisez la propriété `RawPageCount` à la place de la propriété [`PageCount`](../pagecount) pour l'extraction de texte brut. Certains documents ont des numéros de page différents en modes d'extraction de texte précis et brut. La propriété [`PageCount`](../pagecount) peut effectuer des calculs supplémentaires qui impactent la vitesse d'extraction du texte en mode brut.

### Voir aussi

* interface [IDocumentInfo](../../idocumentinfo)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->

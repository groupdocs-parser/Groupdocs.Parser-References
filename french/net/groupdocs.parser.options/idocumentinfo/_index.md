---
title: "IDocumentInfo"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Représente les informations du document."
type: docs
weight: 370
url: /fr/net/groupdocs.parser.options/idocumentinfo/
---

## IDocumentInfo interface

Représente les informations du document.

```csharp
public interface IDocumentInfo
```

## Propriétés

| Nom | Description |
| --- | --- |
| [FileType](../../groupdocs.parser.options/idocumentinfo/filetype) { get; } | Obtient le type du document. |
| [PageCount](../../groupdocs.parser.options/idocumentinfo/pagecount) { get; } | Obtient le nombre total de pages du document. |
| [Pages](../../groupdocs.parser.options/idocumentinfo/pages) { get; } | Obtient les informations sur les pages telles que l’index et la taille de la page. |
| [RawPageCount](../../groupdocs.parser.options/idocumentinfo/rawpagecount) { get; } | Obtient le nombre total de pages brutes du document. |
| [Size](../../groupdocs.parser.options/idocumentinfo/size) { get; } | Obtient la taille du document en octets. |

### Remarques

Les objets qui implémentent cette interface sont renvoyés par la méthode [`GetDocumentInfo`](../../groupdocs.parser/parser/getdocumentinfo). Voir les exemples d’utilisation là‑bas. **En savoir plus:**

* [Get document info](https://docs.groupdocs.com/display/parsernet/Get+document+info)
* [Detect encoding](https://docs.groupdocs.com/display/parsernet/Detect+encoding)

### Voir aussi

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->

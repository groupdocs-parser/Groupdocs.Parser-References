---
title: IDocumentInfo
second_title: Référence de l'API GroupDocs.Parser pour .NET
description: Représente les informations du document.
type: docs
weight: 410
url: /fr/net/groupdocs.parser.options/idocumentinfo/
---
## IDocumentInfo interface

Représente les informations du document.

```csharp
public interface IDocumentInfo
```

## Propriétés

| Nom | La description |
| --- | --- |
| [FileType](../../groupdocs.parser.options/idocumentinfo/filetype) { get; } | Obtient le type de document. |
| [PageCount](../../groupdocs.parser.options/idocumentinfo/pagecount) { get; } | Obtient le nombre total de pages du document. |
| [Pages](../../groupdocs.parser.options/idocumentinfo/pages) { get; } | Obtient les informations sur les pages telles que l'index et la taille de la page. |
| [RawPageCount](../../groupdocs.parser.options/idocumentinfo/rawpagecount) { get; } | Obtient le nombre total de pages brutes du document. |
| [Size](../../groupdocs.parser.options/idocumentinfo/size) { get; } | Obtient la taille du document en octets. |

### Remarques

Les objets qui implémentent cette interface sont retournés par[`GetDocumentInfo`](../../groupdocs.parser/parser/getdocumentinfo) method. Voir les exemples d'utilisation ici. **Apprendre encore plus:**

* [Obtenir des informations sur les documents](https://docs.groupdocs.com/display/parsernet/Get+document+info)
* [Détecter l'encodage](https://docs.groupdocs.com/display/parsernet/Detect+encoding)

### Voir également

* espace de noms [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* Assemblée [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
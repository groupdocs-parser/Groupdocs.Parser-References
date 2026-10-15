---
title: "ContainerItem"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Représente un élément de conteneur tel qu'une entité d'archive Zip, une pièce jointe d'e-mail, un élément de portefeuille PDF, etc."
type: docs
weight: 720
url: /fr/net/groupdocs.parser.data/containeritem/
---

## ContainerItem class

Représente un élément de conteneur tel qu'une entité d'archive Zip, une pièce jointe email, un élément de portefeuille PDF, etc.

```csharp
public sealed class ContainerItem
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Directory](../../groupdocs.parser.data/containeritem/directory) { get; } | Obtient le répertoire de l'élément. |
| [FilePath](../../groupdocs.parser.data/containeritem/filepath) { get; } | Obtient le chemin complet de l'élément. |
| [Metadata](../../groupdocs.parser.data/containeritem/metadata) { get; } | Obtient la collection d'éléments de métadonnées. |
| [Name](../../groupdocs.parser.data/containeritem/name) { get; } | Obtient le nom de l'élément. |
| [Size](../../groupdocs.parser.data/containeritem/size) { get; } | Obtient la taille de l'élément. |

## Méthodes

| Nom | Description |
| --- | --- |
| [DetectFileType](../../groupdocs.parser.data/containeritem/detectfiletype)(FileTypeDetectionMode) | Détecte le type de fichier de l'élément de conteneur. |
| [GetMetadataValue](../../groupdocs.parser.data/containeritem/getmetadatavalue)(string) | Obtient la valeur de la métadonnée. |
| [OpenParser](../../groupdocs.parser.data/containeritem/openparser#openparser)() | Crée l'objet [`Parser`](../../groupdocs.parser/parser) pour le contenu de l'élément. |
| [OpenParser](../../groupdocs.parser.data/containeritem/openparser#openparser_1)(LoadOptions) | Crée l'objet [`Parser`](../../groupdocs.parser/parser) pour le contenu de l'élément avec [`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [OpenParser](../../groupdocs.parser.data/containeritem/openparser#openparser_2)(LoadOptions, ParserSettings) | Crée l'objet [`Parser`](../../groupdocs.parser/parser) pour le contenu de l'élément avec [`LoadOptions`](../../groupdocs.parser.options/loadoptions) et [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [OpenStream](../../groupdocs.parser.data/containeritem/openstream)() | Ouvre le flux du contenu de l'élément. |

### Remarques

Une instance de la classe [`ContainerItem`](../containeritem) est utilisée comme valeur de retour de la méthode [`GetContainer`](../../groupdocs.parser/parser/getcontainer). Voir les exemples d'utilisation là-bas.

### Voir aussi

* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->

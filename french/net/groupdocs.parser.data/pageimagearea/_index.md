---
title: "PageImageArea"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Représente une zone d'image de page utilisée pour représenter une image sur la page dans la fonctionnalité d'analyse par modèle ou une pièce jointe d'image si les images sont extraites des e‑mails ou des archives Zip."
type: docs
weight: 830
url: /fr/net/groupdocs.parser.data/pageimagearea/
---

## PageImageArea class

Représente une zone d'image de page utilisée pour représenter une image sur la page dans la fonctionnalité d'analyse par modèle ou une pièce jointe d'image si les images sont extraites des e‑mails ou des archives Zip.

```csharp
public sealed class PageImageArea : PageArea
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PageImageArea](pageimagearea#constructor)(Stream, FileType, double) | Initialise une nouvelle instance de la classe [`PageImageArea`](../pageimagearea). |
| [PageImageArea](pageimagearea#constructor_1)(Stream, FileType, double, Page, Rectangle) | Initialise une nouvelle instance de la classe [`PageImageArea`](../pageimagearea). |

## Propriétés

| Nom | Description |
| --- | --- |
| [FileType](../../groupdocs.parser.data/pageimagearea/filetype) { get; } | Obtient le format de l'image. |
| [Page](../../groupdocs.parser.data/pagearea/page) { get; } | Obtient les informations de la page du document telles que l'index de page et la taille de page. |
| [Rectangle](../../groupdocs.parser.data/pagearea/rectangle) { get; } | Obtient la zone rectangulaire. |
| [Rotation](../../groupdocs.parser.data/pageimagearea/rotation) { get; } | Obtient l'angle de rotation de l'image. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetImageStream](../../groupdocs.parser.data/pageimagearea/getimagestream#getimagestream)() | Renvoie le flux d'image. |
| [GetImageStream](../../groupdocs.parser.data/pageimagearea/getimagestream#getimagestream_1)(ImageOptions) | Renvoie le flux d'image dans un format différent. |
| [Save](../../groupdocs.parser.data/pageimagearea/save#save)(string) | Enregistre l'image dans le fichier. |
| [Save](../../groupdocs.parser.data/pageimagearea/save#save_1)(string, ImageOptions) | Enregistre l'image dans le fichier dans un format différent. |

### Remarques

Une instance de la classe [`PageImageArea`](../pageimagearea) est utilisée comme valeur de retour des méthodes suivantes :

* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetImages`](../../groupdocs.parser/parser/getimages)

Voir les exemples d'utilisation là-bas.

### Voir aussi

* class [PageArea](../pagearea)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->

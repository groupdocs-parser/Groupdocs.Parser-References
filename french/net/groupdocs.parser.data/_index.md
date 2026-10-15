---
title: "GroupDocs.Parser.Data"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "L'espace de noms fournit des classes qui représentent les résultats d'analyse."
type: docs
weight: 20
url: /fr/net/groupdocs.parser.data/
---

L'espace de noms fournit des classes qui représentent les résultats d'analyse.

## Classes

| Classe | Description |
| --- | --- |
| [AnnotationItem](./annotationitem) | Représente un élément d'annotation qui est utilisé dans la fonctionnalité d'extraction d'annotations. |
| [ContainerItem](./containeritem) | Représente un élément de conteneur tel qu'une entité d'archive Zip, une pièce jointe email, un élément de portefeuille PDF, etc. |
| [DocumentData](./documentdata) | Représente les données du document. Il se compose d'objets [`FieldData`](../groupdocs.parser.data/fielddata) qui contiennent les données de champ du document. |
| [DocumentPageData](./documentpagedata) | Représente les données de la page du document. Il se compose d'objets [`FieldData`](../groupdocs.parser.data/fielddata) qui contiennent les données de champ de la page du document. |
| [FieldData](./fielddata) | Représente les données de champ telles qu'un nom, un indice de page, une valeur de champ, etc. Selon le champ, la valeur peut être un texte, une image, un tableau, etc. |
| [HighlightItem](./highlightitem) | Représente une mise en évidence, une partie du texte généralement utilisée pour expliquer le contexte du texte trouvé dans la fonctionnalité de recherche. |
| [MetadataItem](./metadataitem) | Représente un élément de métadonnées utilisé dans les éléments de conteneur et la fonctionnalité d'extraction de métadonnées. |
| [Page](./page) | Représente les informations de la page du document telles que l'indice de page et la taille de la page. Il est utilisé pour représenter la page qui contient les héritiers de la classe [`PageArea`](../groupdocs.parser.data/pagearea) dans la fonctionnalité d'analyse par modèle. |
| [PageArea](./pagearea) | Représente une classe de base abstraite pour les zones de page utilisées pour représenter des blocs sur la page du document dans la fonctionnalité d'analyse par modèle. |
| [PageBarcodeArea](./pagebarcodearea) | Représente une zone de code-barres de page utilisée pour représenter une valeur de code-barres dans la fonctionnalité d'analyse par modèle. |
| [PageGroupArea](./pagegrouparea) | Représente un groupe de zones de page utilisé pour regrouper différents types de blocs de la page du document dans la fonctionnalité d'analyse par modèle. |
| [PageHyperlinkArea](./pagehyperlinkarea) | Représente une zone de page utilisée pour représenter un hyperlien sur la page. |
| [PageImageArea](./pageimagearea) | Représente une zone d'image de page utilisée pour représenter une image sur la page dans la fonctionnalité d'analyse par modèle ou une pièce jointe d'image si les images sont extraites des e‑mails ou des archives Zip. |
| [PageTableArea](./pagetablearea) | Représente une zone de tableau de page utilisée pour représenter un tableau dans la fonctionnalité d'analyse par modèle. |
| [PageTableAreaCell](./pagetableareacell) | Représente une cellule de tableau utilisée dans la classe [`PageTableArea`](../groupdocs.parser.data/pagetablearea). |
| [PageTextArea](./pagetextarea) | Représente une zone de texte de page utilisée pour représenter une valeur de texte dans la fonctionnalité d'analyse par modèle ou d'analyse de formulaire. |
| [Point](./point) | Représente un point. |
| [Rectangle](./rectangle) | Représente une zone rectangulaire. |
| [SearchResult](./searchresult) | Représente le résultat de la recherche dans la fonctionnalité de recherche. |
| [Size](./size) | Représente une taille. |
| [TextStyle](./textstyle) | Représente le style du texte tel qu'un nom de police, une taille de police, etc. |
| [TocItem](./tocitem) | Représente l'élément utilisé dans la fonctionnalité d'extraction de la table des matières. |
| [WorksheetCell](./worksheetcell) | Représente une cellule de feuille de calcul. |
| [WorksheetInfo](./worksheetinfo) | Représente les informations d'une feuille. |
| [WorksheetRange](./worksheetrange) | Fournit la plage utilisée pour l'extraction de la feuille de calcul. |

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->

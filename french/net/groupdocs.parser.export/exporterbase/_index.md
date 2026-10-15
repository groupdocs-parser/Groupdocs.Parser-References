---
title: "ExporterBase"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Fournit la classe de base pour la fonctionnalité d'exportation des données."
type: docs
weight: 630
url: /fr/net/groupdocs.parser.export/exporterbase/
---

## ExporterBase class

Fournit la classe de base pour la fonctionnalité d'exportation des données.

```csharp
public abstract class ExporterBase
```

## Méthodes

| Nom | Description |
| --- | --- |
| abstract [Export](../../groupdocs.parser.export/exporterbase/export#export)(DocumentData, Stream) | Exporte les données du document vers le flux. |
| [Export](../../groupdocs.parser.export/exporterbase/export#export_1)(DocumentData, string) | Exporte les données du document vers le fichier. |
| abstract [Export](../../groupdocs.parser.export/exporterbase/export#export_2)(IDocumentInfo, Stream) | Exporte les informations du document vers le flux. |
| [Export](../../groupdocs.parser.export/exporterbase/export#export_3)(IDocumentInfo, string) | Exporte les informations du document vers le fichier. |
| abstract [Export](../../groupdocs.parser.export/exporterbase/export#export_4)(IEnumerable&lt;MetadataItem&gt;, Stream) | Exporte la collection de métadonnées vers le flux. |
| [Export](../../groupdocs.parser.export/exporterbase/export#export_5)(IEnumerable&lt;MetadataItem&gt;, string) | Exporte la collection de métadonnées vers le fichier. |
| abstract [Export](../../groupdocs.parser.export/exporterbase/export#export_6)(IEnumerable&lt;PageBarcodeArea&gt;, Stream) | Exporte la collection de codes-barres vers le flux. |
| [Export](../../groupdocs.parser.export/exporterbase/export#export_7)(IEnumerable&lt;PageBarcodeArea&gt;, string) | Exporte la collection de codes-barres vers le fichier. |
| abstract [Export](../../groupdocs.parser.export/exporterbase/export#export_8)(IEnumerable&lt;PageTableArea&gt;, Stream) | Exporte la collection de tableaux vers le flux. |
| [Export](../../groupdocs.parser.export/exporterbase/export#export_9)(IEnumerable&lt;PageTableArea&gt;, string) | Exporte la collection de tableaux vers le fichier. |
| abstract [Export](../../groupdocs.parser.export/exporterbase/export#export_10)(IEnumerable&lt;PageTextArea&gt;, Stream) | Exporte la collection de zones de texte vers le flux. |
| [Export](../../groupdocs.parser.export/exporterbase/export#export_11)(IEnumerable&lt;PageTextArea&gt;, string) | Exporte la collection de zones de texte vers le fichier. |

### Voir aussi

* namespace [GroupDocs.Parser.Export](../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->

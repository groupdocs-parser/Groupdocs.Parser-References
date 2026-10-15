---
title: "JsonExporter"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Fournit la fonctionnalité d'exportation des données au format JSON."
type: docs
weight: 650
url: /fr/net/groupdocs.parser.export/jsonexporter/
---

## JsonExporter class

Fournit la fonctionnalité d'exportation des données au format JSON.

```csharp
public sealed class JsonExporter : ExporterBase
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [JsonExporter](jsonexporter)() | Le constructeur par défaut. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Export](../../groupdocs.parser.export/jsonexporter/export#export)(DocumentData, Stream) | Exporte les données du document vers le flux. |
| [Export](../../groupdocs.parser.export/exporterbase/export)(DocumentData, string) | Exporte les données du document vers le fichier. |
| override [Export](../../groupdocs.parser.export/jsonexporter/export#export_2)(IDocumentInfo, Stream) | Exporte les informations du document vers le flux. |
| [Export](../../groupdocs.parser.export/exporterbase/export)(IDocumentInfo, string) | Exporte les informations du document vers le fichier. |
| override [Export](../../groupdocs.parser.export/jsonexporter/export#export_4)(IEnumerable&lt;MetadataItem&gt;, Stream) | Exporte la collection de métadonnées vers le flux. |
| [Export](../../groupdocs.parser.export/exporterbase/export)(IEnumerable&lt;MetadataItem&gt;, string) | Exporte la collection de métadonnées vers le fichier. |
| override [Export](../../groupdocs.parser.export/jsonexporter/export#export_6)(IEnumerable&lt;PageBarcodeArea&gt;, Stream) | Exporte la collection de codes-barres vers le flux. |
| [Export](../../groupdocs.parser.export/exporterbase/export)(IEnumerable&lt;PageBarcodeArea&gt;, string) | Exporte la collection de codes-barres vers le fichier. |
| override [Export](../../groupdocs.parser.export/jsonexporter/export#export_8)(IEnumerable&lt;PageTableArea&gt;, Stream) | Exporte la collection de tableaux vers le flux. |
| [Export](../../groupdocs.parser.export/exporterbase/export)(IEnumerable&lt;PageTableArea&gt;, string) | Exporte la collection de tableaux vers le fichier. |
| override [Export](../../groupdocs.parser.export/jsonexporter/export#export_10)(IEnumerable&lt;PageTextArea&gt;, Stream) | Exporte la collection de zones de texte vers le flux. |
| [Export](../../groupdocs.parser.export/exporterbase/export)(IEnumerable&lt;PageTextArea&gt;, string) | Exporte la collection de zones de texte vers le fichier. |

### Voir aussi

* class [ExporterBase](../exporterbase)
* namespace [GroupDocs.Parser.Export](../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->

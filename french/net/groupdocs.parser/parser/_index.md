---
title: "Analyseur"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Représente la classe principale qui contrôle l'extraction du conteneur d'images texte et la fonctionnalité d'analyse."
type: docs
weight: 30
url: /fr/net/groupdocs.parser/parser/
---

## Parser class

Représente la classe principale qui contrôle le texte, les images, l'extraction de conteneurs et la fonctionnalité d'analyse.

```csharp
public sealed class Parser : IDisposable
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | Initialise une nouvelle instance de la classe [`Parser`](../parser) pour extraire des données d'une base de données. |
| [Parser](parser#constructor)(EmailConnection) | Initialise une nouvelle instance de la classe [`Parser`](../parser) pour extraire des données d'un serveur de messagerie distant. |
| [Parser](parser#constructor_4)(Stream) | Initialise une nouvelle instance de la classe [`Parser`](../parser). |
| [Parser](parser#constructor_8)(string) | Initialise une nouvelle instance de la classe [`Parser`](../parser). |
| [Parser](parser#constructor_12)(Uri) | Initialise une nouvelle instance de la classe [`Parser`](../parser) pour extraire des données d'une URI. |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | Initialise une nouvelle instance de la classe [`Parser`](../parser) pour extraire des données d'une base de données. |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | Initialise une nouvelle instance de la classe [`Parser`](../parser) pour extraire des données d'un serveur de messagerie distant. |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | Initialise une nouvelle instance de la classe [`Parser`](../parser) avec [`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [Parser](parser#constructor_7)(Stream, ParserSettings) | Initialise une nouvelle instance de la classe [`Parser`](../parser) avec [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_9)(string, LoadOptions) | Initialise une nouvelle instance de la classe [`Parser`](../parser) avec [`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [Parser](parser#constructor_11)(string, ParserSettings) | Initialise une nouvelle instance de la classe [`Parser`](../parser) avec [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_13)(Uri, LoadOptions) | Initialise une nouvelle instance de la classe [`Parser`](../parser) pour extraire des données d'une URI avec *loadOptions*. |
| [Parser](parser#constructor_15)(Uri, ParserSettings) | Initialise une nouvelle instance de la classe [`Parser`](../parser) pour extraire des données d'une URI avec *parserSettings*. |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | Initialise une nouvelle instance de la classe [`Parser`](../parser) avec [`LoadOptions`](../../groupdocs.parser.options/loadoptions) et [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_10)(string, LoadOptions, ParserSettings) | Initialise une nouvelle instance de la classe [`Parser`](../parser) avec [`LoadOptions`](../../groupdocs.parser.options/loadoptions) et [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_14)(Uri, LoadOptions, ParserSettings) | Initialise une nouvelle instance de la classe [`Parser`](../parser) pour extraire des données d'une URI avec *loadOptions* et *parserSettings*. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | Obtient les fonctionnalités prises en charge. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | Effectue les tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées. |
| [GenerateAdjustmentFields](../../groupdocs.parser/parser/generateadjustmentfields)(AdjustmentFieldsOptions) | Génère des champs pour l'ajustement automatique de la position et de l'échelle du modèle. |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | Obtenir un aperçu des pages. |
| [GetAnnotations](../../groupdocs.parser/parser/getannotations#getannotations)() | Extrait les annotations du document. Notez que seul le format PDF est actuellement pris en charge. |
| [GetAnnotations](../../groupdocs.parser/parser/getannotations#getannotations_1)(int) | Extrait les annotations de la page du document. Notez que seul le format PDF est actuellement pris en charge. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | Extrait les codes-barres du document. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(BarcodeOptions) | Extrait les codes-barres du document en utilisant des options de personnalisation. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int) | Extrait les codes-barres de la page du document. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_4)(int, BarcodeOptions) | Extrait les codes-barres de la page du document en utilisant des options de personnalisation. |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | Extrait un objet conteneur du document pour travailler avec des formats contenant des pièces jointes, des archives ZIP, etc. |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | Renvoie les informations générales sur le document. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | Extrait un texte formaté du document. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | Extrait un texte formaté de la page du document. |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | Extrait une mise en évidence du document. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | Extrait les hyperliens du document. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | Extrait les hyperliens de la page du document. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | Extrait les hyperliens du document en utilisant des options de personnalisation (pour définir la zone rectangulaire contenant les hyperliens). |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | Extrait les hyperliens de la page du document en utilisant des options de personnalisation (pour définir la zone rectangulaire contenant les hyperliens). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | Extrait les images du document. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | Extrait les images de la page du document. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | Extrait les images du document en utilisant des options de personnalisation (pour définir la zone rectangulaire contenant les images). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | Extrait les images de la page du document en utilisant des options de personnalisation (pour définir la zone rectangulaire contenant les images). |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | Extrait les métadonnées du document. |
| [GetPagePreview](../../groupdocs.parser/parser/getpagepreview#getpagepreview)(int) | Génère un aperçu de la page du document. |
| [GetPagePreview](../../groupdocs.parser/parser/getpagepreview#getpagepreview_1)(int, PagePreviewOptions) | Génère un aperçu de la page du document en utilisant des options de personnalisation. |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | Extrait un texte structuré du document. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)() | Extrait les tableaux du document. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_2)(int) | Extrait les tableaux de la page du document. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(PageTableAreaOptions) | Extrait les tableaux du document. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_3)(int, PageTableAreaOptions) | Extrait les tableaux de la page du document. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | Extrait un texte du document. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | Extrait un texte de la page du document. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | Extrait une page de texte du document en utilisant les options de texte (pour activer le mode d'extraction de texte brut rapide). |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | Extrait un texte de la page du document en utilisant les options de texte (pour activer le mode d'extraction de texte brut rapide). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | Extrait les zones de texte du document. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | Extrait les zones de texte de la page du document. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | Extrait les zones de texte du document en utilisant des options de personnalisation (expression régulière, respect de la casse, etc.). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | Extrait les zones de texte de la page du document en utilisant des options de personnalisation (expression régulière, respect de la casse, etc.). |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | Extrait une table des matières du document. |
| [GetWorksheetCells](../../groupdocs.parser/parser/getworksheetcells#getworksheetcells)(int) | Extrait les cellules de la feuille de calcul. |
| [GetWorksheetCells](../../groupdocs.parser/parser/getworksheetcells#getworksheetcells_1)(int, WorksheetOptions) | Extrait les cellules de la feuille de calcul en utilisant des options de personnalisation. |
| [GetWorksheetInfo](../../groupdocs.parser/parser/getworksheetinfo#getworksheetinfo_1)() | Extrait les informations sur toutes les feuilles de calcul du classeur. |
| [GetWorksheetInfo](../../groupdocs.parser/parser/getworksheetinfo#getworksheetinfo)(int) | Extrait les informations sur la feuille de calcul. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate)(Template) | Analyse le document à l'aide du modèle généré par l'utilisateur. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate_1)(Template, ParseByTemplateOptions) | Analyse le document à l'aide du modèle généré par l'utilisateur en utilisant des options de personnalisation. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate_2)(TemplateCollection, ParseByTemplateOptions) | Sélectionne le modèle le plus adapté parmi la collection fournie, puis analyse le document selon le modèle sélectionné. |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | Analyse le formulaire du document. |
| [Search](../../groupdocs.parser/parser/search#search)(string) | Recherche un *mot‑clé* dans le document. |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | Recherche un *mot‑clé* dans le document en utilisant des options de recherche (expression régulière, respect de la casse, etc.). |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | Renvoie les informations générales sur un fichier. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | Renvoie les informations générales sur un fichier. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | Renvoie les informations générales sur un fichier. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | Renvoie les informations générales sur un fichier. |

### Voir aussi

* namespace [GroupDocs.Parser](../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->

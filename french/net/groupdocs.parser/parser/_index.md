---
title: Parser
second_title: Référence de l'API GroupDocs.Parser pour .NET
description: Représente la classe principale qui contrôle le texte les images lextraction de conteneurs et la fonctionnalité danalyse.
type: docs
weight: 640
url: /fr/net/groupdocs.parser/parser/
---
## Parser class

Représente la classe principale qui contrôle le texte, les images, l'extraction de conteneurs et la fonctionnalité d'analyse.

```csharp
public sealed class Parser : IDisposable
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | Initialise une nouvelle instance du[`Parser`](../parser) classe pour extraire des données d'une base de données. |
| [Parser](parser#constructor)(EmailConnection) | Initialise une nouvelle instance du[`Parser`](../parser) classe pour extraire les données d'un serveur de messagerie distant. |
| [Parser](parser#constructor_4)(Stream) | Initialise une nouvelle instance du[`Parser`](../parser) classe. |
| [Parser](parser#constructor_8)(string) | Initialise une nouvelle instance du[`Parser`](../parser) classe. |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | Initialise une nouvelle instance du[`Parser`](../parser) classe pour extraire des données d'une base de données. |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | Initialise une nouvelle instance du[`Parser`](../parser) classe pour extraire les données d'un serveur de messagerie distant. |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | Initialise une nouvelle instance du[`Parser`](../parser) classe avec[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_7)(Stream, ParserSettings) | Initialise une nouvelle instance du[`Parser`](../parser) classe avec[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_9)(string, LoadOptions) | Initialise une nouvelle instance du[`Parser`](../parser) classe avec[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_11)(string, ParserSettings) | Initialise une nouvelle instance du[`Parser`](../parser) classe avec[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | Initialise une nouvelle instance du[`Parser`](../parser) classe avec[`LoadOptions`](../../groupdocs.parser.options/loadoptions) et[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_10)(string, LoadOptions, ParserSettings) | Initialise une nouvelle instance du[`Parser`](../parser) classe avec[`LoadOptions`](../../groupdocs.parser.options/loadoptions) et[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |

## Propriétés

| Nom | La description |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | Obtient les fonctionnalités prises en charge. |

## Méthodes

| Nom | La description |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | Effectue des tâches définies par l'application associées à la libération, à la libération ou à la réinitialisation des ressources non gérées. |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | Obtenir un aperçu des pages. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | Extrait les codes-barres du document. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_2)(int) | Extrait les codes-barres de la page du document. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(PageAreaOptions) | Extrait les codes-barres du document à l'aide des options de personnalisation (pour définir la zone rectangulaire contenant les codes-barres). |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int, PageAreaOptions) | Extrait les codes-barres de la page du document à l'aide des options de personnalisation (pour définir la zone rectangulaire contenant les codes-barres). |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | Extrait un objet conteneur du document pour travailler avec des formats contenant des pièces jointes, des archives ZIP, etc. |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | Renvoie les informations générales sur le document. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | Extrait un texte formaté du document. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | Extrait un texte formaté de la page du document. |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | Extrait une surbrillance du document. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | Extrait les hyperliens du document. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | Extrait les hyperliens de la page du document. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | Extrait les hyperliens du document à l'aide des options de personnalisation (pour définir la zone rectangulaire contenant les hyperliens). |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | Extrait les hyperliens de la page du document à l'aide des options de personnalisation (pour définir la zone rectangulaire contenant les hyperliens). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | Extrait les images du document. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | Extrait les images de la page du document. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | Extrait les images du document à l'aide des options de personnalisation (pour définir la zone rectangulaire contenant les images). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | Extrait les images de la page du document à l'aide des options de personnalisation (pour définir la zone rectangulaire contenant les images). |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | Extrait les métadonnées du document. |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | Extrait un texte structuré du document. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)(PageTableAreaOptions) | Extrait les tableaux du document. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(int, PageTableAreaOptions) | Extrait les tableaux de la page du document. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | Extrait un texte du document. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | Extrait un texte de la page du document. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | Extrait une page de texte du document à l'aide des options de texte (pour activer le mode d'extraction rapide de texte brut). |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | Extrait un texte de la page du document à l'aide des options de texte (pour activer le mode d'extraction rapide de texte brut). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | Extrait des zones de texte du document. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | Extrait les zones de texte de la page du document. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | Extrait des zones de texte du document à l'aide d'options de personnalisation (expression régulière, correspondance de casse, etc.). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | Extrait des zones de texte de la page du document à l'aide d'options de personnalisation (expression régulière, correspondance de casse, etc.). |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | Extrait une table des matières du document. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate)(Template) | Analyse le document par le modèle généré par l'utilisateur. |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | Analyse le formulaire de document. |
| [Search](../../groupdocs.parser/parser/search#search)(string) | Recherche un*keyword* dans le document. |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | Recherche un*keyword*dans le document à l'aide des options de recherche (expression régulière, correspondance de casse, etc.). |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | Renvoie les informations générales sur un fichier. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | Renvoie les informations générales sur un fichier. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | Renvoie les informations générales sur un fichier. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | Renvoie les informations générales sur un fichier. |

### Voir également

* espace de noms [GroupDocs.Parser](../../groupdocs.parser)
* Assemblée [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

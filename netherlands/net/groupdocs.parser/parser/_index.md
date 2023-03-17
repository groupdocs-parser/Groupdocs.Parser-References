---
title: Parser
second_title: GroupDocs.Parser voor .NET API-referentie
description: Vertegenwoordigt de hoofdklasse die tekst afbeeldingen containerextractie en parseerfunctionaliteit bestuurt.
type: docs
weight: 640
url: /nl/net/groupdocs.parser/parser/
---
## Parser class

Vertegenwoordigt de hoofdklasse die tekst, afbeeldingen, containerextractie en parseerfunctionaliteit bestuurt.

```csharp
public sealed class Parser : IDisposable
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | Initialiseert een nieuw exemplaar van het[`Parser`](../parser) klasse om gegevens uit een database te extraheren. |
| [Parser](parser#constructor)(EmailConnection) | Initialiseert een nieuw exemplaar van het[`Parser`](../parser) class om gegevens te extraheren van een externe e-mailserver. |
| [Parser](parser#constructor_4)(Stream) | Initialiseert een nieuw exemplaar van het[`Parser`](../parser) klasse. |
| [Parser](parser#constructor_8)(string) | Initialiseert een nieuw exemplaar van het[`Parser`](../parser) klasse. |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | Initialiseert een nieuw exemplaar van het[`Parser`](../parser) klasse om gegevens uit een database te extraheren. |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | Initialiseert een nieuw exemplaar van het[`Parser`](../parser) class om gegevens te extraheren van een externe e-mailserver. |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | Initialiseert een nieuw exemplaar van het[`Parser`](../parser) klas mee[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_7)(Stream, ParserSettings) | Initialiseert een nieuw exemplaar van het[`Parser`](../parser) klas mee[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_9)(string, LoadOptions) | Initialiseert een nieuw exemplaar van het[`Parser`](../parser) klas mee[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_11)(string, ParserSettings) | Initialiseert een nieuw exemplaar van het[`Parser`](../parser) klas mee[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | Initialiseert een nieuw exemplaar van het[`Parser`](../parser) klas mee[`LoadOptions`](../../groupdocs.parser.options/loadoptions) en[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_10)(string, LoadOptions, ParserSettings) | Initialiseert een nieuw exemplaar van het[`Parser`](../parser) klas mee[`LoadOptions`](../../groupdocs.parser.options/loadoptions) en[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | Krijgt de ondersteunde functies. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | Voert door de toepassing gedefinieerde taken uit die verband houden met het vrijmaken, vrijgeven of resetten van onbeheerde bronnen. |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | Paginavoorbeeld ophalen. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | Haalt streepjescodes uit het document. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_2)(int) | Haalt streepjescodes uit de documentpagina. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(PageAreaOptions) | Haalt streepjescodes uit het document met behulp van aanpassingsopties (om het rechthoekige gebied in te stellen dat streepjescodes bevat). |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int, PageAreaOptions) | Haalt streepjescodes uit de documentpagina met behulp van aanpassingsopties (om het rechthoekige gebied in te stellen dat streepjescodes bevat). |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | Haalt een containerobject uit het document om te werken met indelingen die bijlagen, ZIP-archieven etc. bevatten |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | Retourneert de algemene informatie over het document. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | Extraheert een opgemaakte tekst uit het document. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | Extraheert een opgemaakte tekst van de documentpagina. |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | Haalt een markering uit het document. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | Haalt hyperlinks uit het document. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | Haalt hyperlinks uit de documentpagina. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | Haalt hyperlinks uit het document met behulp van aanpassingsopties (om het rechthoekige gebied in te stellen dat hyperlinks bevat). |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | Haalt hyperlinks uit de documentpagina met behulp van aanpassingsopties (om het rechthoekige gebied in te stellen dat hyperlinks bevat). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | Haalt afbeeldingen uit het document. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | Haalt afbeeldingen uit de documentpagina. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | Haalt afbeeldingen uit het document met behulp van aanpassingsopties (om het rechthoekige gebied in te stellen dat afbeeldingen bevat). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | Haalt afbeeldingen uit de documentpagina met behulp van aanpassingsopties (om het rechthoekige gebied in te stellen dat afbeeldingen bevat). |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | Haalt metadata uit het document. |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | Haalt een gestructureerde tekst uit het document. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)(PageTableAreaOptions) | Haalt tabellen uit het document. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(int, PageTableAreaOptions) | Haalt tabellen uit de documentpagina. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | Extraheert een tekst uit het document. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | Extraheert een tekst van de documentpagina. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | Extraheert een tekstpagina uit het document met behulp van tekstopties (om de modus Raw Fast Text Extraction in te schakelen). |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | Extraheert een tekst van de documentpagina met behulp van tekstopties (om de modus Raw Fast Text Extraction in te schakelen). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | Extraheert tekstgebieden uit het document. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | Extraheert tekstgebieden van de documentpagina. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | Extraheert tekstgebieden uit het document met behulp van aanpassingsopties (reguliere expressie, hoofdletters, enz.). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | Extraheert tekstgebieden van de documentpagina met behulp van aanpassingsopties (reguliere expressie, hoofdletters, enz.). |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | Haalt een inhoudsopgave uit het document. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate)(Template) | Parseert het document door de door de gebruiker gegenereerde sjabloon. |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | Parseert het documentformulier. |
| [Search](../../groupdocs.parser/parser/search#search)(string) | Zoekt een*keyword* in het document. |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | Zoekt een*keyword*in het document met behulp van zoekopties (reguliere expressie, hoofdlettergebruik, etc.). |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | Retourneert de algemene informatie over een bestand. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | Retourneert de algemene informatie over een bestand. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | Retourneert de algemene informatie over een bestand. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | Retourneert de algemene informatie over een bestand. |

### Zie ook

* naamruimte [GroupDocs.Parser](../../groupdocs.parser)
* montage [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

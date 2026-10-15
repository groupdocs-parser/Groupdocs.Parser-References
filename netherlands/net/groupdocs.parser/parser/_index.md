---
title: "Parser"
second_title: "GroupDocs.Parser voor .NET API-referentie"
description: "Stelt de hoofdklasse voor die de extractie van tekstafbeeldingscontainers en de parserfunctionaliteit beheert."
type: docs
weight: 30
url: /nl/net/groupdocs.parser/parser/
---

## Parser class

Stelt de hoofdklasse voor die tekst, afbeeldingen, containerextractie en ontleedfunctionaliteit beheert.

```csharp
public sealed class Parser : IDisposable
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | Initialiseert een nieuw exemplaar van de [`Parser`](../parser) klasse om gegevens uit een database te extraheren. |
| [Parser](parser#constructor)(EmailConnection) | Initialiseert een nieuw exemplaar van de [`Parser`](../parser) klasse om gegevens van een externe e-mailserver te extraheren. |
| [Parser](parser#constructor_4)(Stream) | Initialiseert een nieuw exemplaar van de [`Parser`](../parser) klasse. |
| [Parser](parser#constructor_8)(string) | Initialiseert een nieuw exemplaar van de [`Parser`](../parser) klasse. |
| [Parser](parser#constructor_12)(Uri) | Initialiseert een nieuw exemplaar van de [`Parser`](../parser) klasse om gegevens van een URI te extraheren. |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | Initialiseert een nieuw exemplaar van de [`Parser`](../parser) klasse om gegevens uit een database te extraheren. |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | Initialiseert een nieuw exemplaar van de [`Parser`](../parser) klasse om gegevens van een externe e-mailserver te extraheren. |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | Initialiseert een nieuw exemplaar van de [`Parser`](../parser) klasse met [`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [Parser](parser#constructor_7)(Stream, ParserSettings) | Initialiseert een nieuw exemplaar van de [`Parser`](../parser) klasse met [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_9)(string, LoadOptions) | Initialiseert een nieuw exemplaar van de [`Parser`](../parser) klasse met [`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [Parser](parser#constructor_11)(string, ParserSettings) | Initialiseert een nieuw exemplaar van de [`Parser`](../parser) klasse met [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_13)(Uri, LoadOptions) | Initialiseert een nieuw exemplaar van de [`Parser`](../parser) klasse om gegevens van een URI te extraheren met *loadOptions*. |
| [Parser](parser#constructor_15)(Uri, ParserSettings) | Initialiseert een nieuw exemplaar van de [`Parser`](../parser) klasse om gegevens van een URI te extraheren met *parserSettings*. |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | Initialiseert een nieuw exemplaar van de [`Parser`](../parser) klasse met [`LoadOptions`](../../groupdocs.parser.options/loadoptions) en [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_10)(string, LoadOptions, ParserSettings) | Initialiseert een nieuw exemplaar van de [`Parser`](../parser) klasse met [`LoadOptions`](../../groupdocs.parser.options/loadoptions) en [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_14)(Uri, LoadOptions, ParserSettings) | Initialiseert een nieuw exemplaar van de [`Parser`](../parser) klasse om gegevens van een URI te extraheren met *loadOptions* en *parserSettings*. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | Haalt de ondersteunde functies op. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | Voert door de applicatie gedefinieerde taken uit die verband houden met het vrijgeven, loslaten of opnieuw instellen van niet-beheerde resources. |
| [GenerateAdjustmentFields](../../groupdocs.parser/parser/generateadjustmentfields)(AdjustmentFieldsOptions) | Genereert velden voor automatische aanpassing van de sjabloonpositie en schaal. |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | Bekijk een voorbeeld van pagina's. |
| [GetAnnotations](../../groupdocs.parser/parser/getannotations#getannotations)() | Extraheert annotaties uit het document. Merk op dat momenteel alleen PDF-indeling wordt ondersteund. |
| [GetAnnotations](../../groupdocs.parser/parser/getannotations#getannotations_1)(int) | Extraheert annotaties van de documentpagina. Merk op dat momenteel alleen PDF-indeling wordt ondersteund. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | Extraheert barcodes uit het document. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(BarcodeOptions) | Extraheert barcodes uit het document met behulp van aanpassingsopties. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int) | Extraheert barcodes van de documentpagina. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_4)(int, BarcodeOptions) | Extraheert barcodes van de documentpagina met behulp van aanpassingsopties. |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | Extraheert een containerobject uit het document om te werken met indelingen die bijlagen, ZIP-archieven enz. bevatten. |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | Geeft de algemene informatie over het document terug. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | Extraheert een opgemaakte tekst uit het document. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | Extraheert een opgemaakte tekst van de documentpagina. |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | Extraheert een markering uit het document. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | Extraheert hyperlinks uit het document. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | Extraheert hyperlinks van de documentpagina. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | Extraheert hyperlinks uit het document met behulp van aanpassingsopties (om het rechthoekige gebied dat hyperlinks bevat in te stellen). |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | Extraheert hyperlinks van de documentpagina met behulp van aanpassingsopties (om het rechthoekige gebied dat hyperlinks bevat in te stellen). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | Extraheert afbeeldingen uit het document. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | Extraheert afbeeldingen van de documentpagina. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | Extraheert afbeeldingen uit het document met behulp van aanpassingsopties (om het rechthoekige gebied dat afbeeldingen bevat in te stellen). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | Extraheert afbeeldingen van de documentpagina met behulp van aanpassingsopties (om het rechthoekige gebied dat afbeeldingen bevat in te stellen). |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | Extraheert metadata uit het document. |
| [GetPagePreview](../../groupdocs.parser/parser/getpagepreview#getpagepreview)(int) | Genereert een voorbeeld van een documentpagina. |
| [GetPagePreview](../../groupdocs.parser/parser/getpagepreview#getpagepreview_1)(int, PagePreviewOptions) | Genereert een voorbeeld van een documentpagina met behulp van aanpassingsopties. |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | Extraheert een gestructureerde tekst uit het document. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)() | Extraheert tabellen uit het document. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_2)(int) | Extraheert tabellen van de documentpagina. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(PageTableAreaOptions) | Extraheert tabellen uit het document. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_3)(int, PageTableAreaOptions) | Extraheert tabellen van de documentpagina. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | Extraheert een tekst uit het document. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | Extraheert een tekst van de documentpagina. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | Extraheert een tekspagina uit het document met behulp van tekstopties (om de ruwe snelle tekstelextractiemodus in te schakelen). |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | Extraheert een tekst van de documentpagina met behulp van tekstopties (om de ruwe snelle tekstelextractiemodus in te schakelen). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | Extraheert tekstgebieden uit het document. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | Extraheert tekstgebieden van de documentpagina. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | Extraheert tekstgebieden uit het document met behulp van aanpassingsopties (reguliere expressie, hoofdlettergevoeligheid, enz.). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | Extraheert tekstgebieden van de documentpagina met behulp van aanpassingsopties (reguliere expressie, hoofdlettergevoeligheid, enz.). |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | Extraheert een inhoudsopgave uit het document. |
| [GetWorksheetCells](../../groupdocs.parser/parser/getworksheetcells#getworksheetcells)(int) | Extraheert werkbladcellen. |
| [GetWorksheetCells](../../groupdocs.parser/parser/getworksheetcells#getworksheetcells_1)(int, WorksheetOptions) | Extraheert werkbladcellen met behulp van aanpassingsopties. |
| [GetWorksheetInfo](../../groupdocs.parser/parser/getworksheetinfo#getworksheetinfo_1)() | Extraheert de informatie over alle werkbladen in de spreadsheet. |
| [GetWorksheetInfo](../../groupdocs.parser/parser/getworksheetinfo#getworksheetinfo)(int) | Extraheert de informatie over het werkblad. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate)(Template) | Parseert het document met behulp van de door de gebruiker gegenereerde sjabloon. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate_1)(Template, ParseByTemplateOptions) | Parseert het document met behulp van de door de gebruiker gegenereerde sjabloon en aanpassingsopties. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate_2)(TemplateCollection, ParseByTemplateOptions) | Selecteert het meest geschikte sjabloon uit de verstrekte collectie en parseert vervolgens het document met het geselecteerde sjabloon. |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | Parseert het documentformulier. |
| [Search](../../groupdocs.parser/parser/search#search)(string) | Zoekt een *keyword* in het document. |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | Zoekt een *keyword* in het document met behulp van zoekopties (reguliere expressie, hoofdlettergevoeligheid, enz.). |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | Retourneert de algemene informatie over een bestand. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | Retourneert de algemene informatie over een bestand. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | Retourneert de algemene informatie over een bestand. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | Retourneert de algemene informatie over een bestand. |

### Zie ook

* namespace [GroupDocs.Parser](../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

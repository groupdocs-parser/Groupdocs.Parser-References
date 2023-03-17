---
title: Parser
second_title: GroupDocs.Parser för .NET API-referens
description: Representerar huvudklassen som styr text bilder containerextraktion och analysfunktioner.
type: docs
weight: 640
url: /sv/net/groupdocs.parser/parser/
---
## Parser class

Representerar huvudklassen som styr text, bilder, containerextraktion och analysfunktioner.

```csharp
public sealed class Parser : IDisposable
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | Initierar en ny instans av[`Parser`](../parser) klass för att extrahera data från en databas. |
| [Parser](parser#constructor)(EmailConnection) | Initierar en ny instans av[`Parser`](../parser) klass för att extrahera data från en fjärransluten e-postserver. |
| [Parser](parser#constructor_4)(Stream) | Initierar en ny instans av[`Parser`](../parser) class. |
| [Parser](parser#constructor_8)(string) | Initierar en ny instans av[`Parser`](../parser) class. |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | Initierar en ny instans av[`Parser`](../parser) klass för att extrahera data från en databas. |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | Initierar en ny instans av[`Parser`](../parser) klass för att extrahera data från en fjärransluten e-postserver. |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | Initierar en ny instans av[`Parser`](../parser) klass med[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_7)(Stream, ParserSettings) | Initierar en ny instans av[`Parser`](../parser) klass med[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_9)(string, LoadOptions) | Initierar en ny instans av[`Parser`](../parser) klass med[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_11)(string, ParserSettings) | Initierar en ny instans av[`Parser`](../parser) klass med[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | Initierar en ny instans av[`Parser`](../parser) klass med[`LoadOptions`](../../groupdocs.parser.options/loadoptions) och[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_10)(string, LoadOptions, ParserSettings) | Initierar en ny instans av[`Parser`](../parser) klass med[`LoadOptions`](../../groupdocs.parser.options/loadoptions) och[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | Får de funktioner som stöds. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | Utför programdefinierade uppgifter associerade med att frigöra, frigöra eller återställa ohanterade resurser. |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | Få förhandsgranskning av sidor. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | Extraherar streckkoder från dokumentet. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_2)(int) | Extraherar streckkoder från dokumentsidan. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(PageAreaOptions) | Extraherar streckkoder från dokumentet med hjälp av anpassningsalternativ (för att ställa in det rektangulära område som innehåller streckkoder). |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int, PageAreaOptions) | Extraherar streckkoder från dokumentsidan med hjälp av anpassningsalternativ (för att ställa in det rektangulära område som innehåller streckkoder). |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | Extraherar ett containerobjekt från dokumentet för att arbeta med format som innehåller bilagor, ZIP-arkiv etc. |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | Returnerar den allmänna informationen om dokumentet. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | Extraherar en formaterad text från dokumentet. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | Extraherar en formaterad text från dokumentsidan. |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | Extraherar en markering från dokumentet. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | Extraherar hyperlänkar från dokumentet. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | Extraherar hyperlänkar från dokumentsidan. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | Extraherar hyperlänkar från dokumentet med hjälp av anpassningsalternativ (för att ställa in det rektangulära område som innehåller hyperlänkar). |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | Extraherar hyperlänkar från dokumentsidan med hjälp av anpassningsalternativ (för att ställa in det rektangulära område som innehåller hyperlänkar). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | Extraherar bilder från dokumentet. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | Extraherar bilder från dokumentsidan. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | Extraherar bilder från dokumentet med hjälp av anpassningsalternativ (för att ställa in det rektangulära område som innehåller bilder). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | Extraherar bilder från dokumentsidan med hjälp av anpassningsalternativ (för att ställa in det rektangulära område som innehåller bilder). |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | Extraherar metadata från dokumentet. |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | Extraherar en strukturerad text från dokumentet. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)(PageTableAreaOptions) | Extraherar tabeller från dokumentet. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(int, PageTableAreaOptions) | Extraherar tabeller från dokumentsidan. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | Extraherar en text från dokumentet. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | Extraherar en text från dokumentsidan. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | Extraherar en textsida från dokumentet med hjälp av textalternativ (för att aktivera läget för rå textextrahering). |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | Extraherar en text från dokumentsidan med hjälp av textalternativ (för att aktivera råsnabbt textextraktionsläge). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | Extraherar textområden från dokumentet. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | Extraherar textområden från dokumentsidan. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | Extraherar textområden från dokumentet med hjälp av anpassningsalternativ (reguljärt uttryck, skiftläge, etc.). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | Extraherar textområden från dokumentsidan med hjälp av anpassningsalternativ (reguljärt uttryck, skiftläge, etc.). |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | Extraherar en innehållsförteckning från dokumentet. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate)(Template) | Analyserar dokumentet med den användargenererade mallen. |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | Analyserar dokumentformuläret. |
| [Search](../../groupdocs.parser/parser/search#search)(string) | Söker a*keyword* i dokumentet. |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | Söker a*keyword* dokumentet med hjälp av sökalternativ (reguljärt uttryck, matcha skiftläge, etc.). |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | Returnerar den allmänna informationen om en fil. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | Returnerar den allmänna informationen om en fil. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | Returnerar den allmänna informationen om en fil. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | Returnerar den allmänna informationen om en fil. |

### Se även

* namnutrymme [GroupDocs.Parser](../../groupdocs.parser)
* hopsättning [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

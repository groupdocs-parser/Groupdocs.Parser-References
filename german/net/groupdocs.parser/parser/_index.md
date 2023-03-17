---
title: Parser
second_title: GroupDocs.Parser für .NET-API-Referenz
description: Stellt die Hauptklasse dar die Text Bilder Containerextraktion und ParsingFunktionalität steuert.
type: docs
weight: 640
url: /de/net/groupdocs.parser/parser/
---
## Parser class

Stellt die Hauptklasse dar, die Text, Bilder, Containerextraktion und Parsing-Funktionalität steuert.

```csharp
public sealed class Parser : IDisposable
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | Initialisiert eine neue Instanz von[`Parser`](../parser) Klasse zum Extrahieren von Daten aus einer Datenbank. |
| [Parser](parser#constructor)(EmailConnection) | Initialisiert eine neue Instanz von[`Parser`](../parser) Klasse zum Extrahieren von Daten von einem Remote-E-Mail-Server. |
| [Parser](parser#constructor_4)(Stream) | Initialisiert eine neue Instanz von[`Parser`](../parser) Klasse. |
| [Parser](parser#constructor_8)(string) | Initialisiert eine neue Instanz von[`Parser`](../parser) Klasse. |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | Initialisiert eine neue Instanz von[`Parser`](../parser) Klasse zum Extrahieren von Daten aus einer Datenbank. |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | Initialisiert eine neue Instanz von[`Parser`](../parser) Klasse zum Extrahieren von Daten von einem Remote-E-Mail-Server. |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | Initialisiert eine neue Instanz von[`Parser`](../parser) Klasse mit[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_7)(Stream, ParserSettings) | Initialisiert eine neue Instanz von[`Parser`](../parser) Klasse mit[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_9)(string, LoadOptions) | Initialisiert eine neue Instanz von[`Parser`](../parser) Klasse mit[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_11)(string, ParserSettings) | Initialisiert eine neue Instanz von[`Parser`](../parser) Klasse mit[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | Initialisiert eine neue Instanz von[`Parser`](../parser) Klasse mit[`LoadOptions`](../../groupdocs.parser.options/loadoptions) und[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_10)(string, LoadOptions, ParserSettings) | Initialisiert eine neue Instanz von[`Parser`](../parser) Klasse mit[`LoadOptions`](../../groupdocs.parser.options/loadoptions) und[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | Ruft die unterstützten Funktionen ab. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | Führt anwendungsdefinierte Aufgaben aus, die mit dem Freigeben, Freigeben oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | Seitenvorschau abrufen. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | Extrahiert Barcodes aus dem Dokument. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_2)(int) | Extrahiert Barcodes von der Dokumentseite. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(PageAreaOptions) | Extrahiert Barcodes aus dem Dokument mithilfe der Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Barcodes enthält). |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int, PageAreaOptions) | Extrahiert Barcodes von der Dokumentseite mithilfe von Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Barcodes enthält). |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | Extrahiert ein Containerobjekt aus dem Dokument, um mit Formaten zu arbeiten, die Anhänge, ZIP-Archive usw. enthalten. |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | Gibt die allgemeinen Informationen zum Dokument zurück. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | Extrahiert einen formatierten Text aus dem Dokument. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | Extrahiert einen formatierten Text aus der Dokumentseite. |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | Extrahiert eine Markierung aus dem Dokument. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | Extrahiert Hyperlinks aus dem Dokument. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | Extrahiert Hyperlinks von der Dokumentseite. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | Extrahiert Hyperlinks aus dem Dokument mithilfe von Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Hyperlinks enthält). |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | Extrahiert Hyperlinks von der Dokumentseite mithilfe von Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Hyperlinks enthält). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | Extrahiert Bilder aus dem Dokument. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | Extrahiert Bilder von der Dokumentseite. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | Extrahiert Bilder aus dem Dokument mithilfe der Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Bilder enthält). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | Extrahiert Bilder von der Dokumentseite mit Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Bilder enthält). |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | Extrahiert Metadaten aus dem Dokument. |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | Extrahiert einen strukturierten Text aus dem Dokument. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)(PageTableAreaOptions) | Extrahiert Tabellen aus dem Dokument. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(int, PageTableAreaOptions) | Extrahiert Tabellen von der Dokumentseite. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | Extrahiert einen Text aus dem Dokument. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | Extrahiert einen Text aus der Dokumentseite. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | Extrahiert eine Textseite aus dem Dokument mithilfe von Textoptionen (um den Rohtext-Schnellextraktionsmodus zu aktivieren). |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | Extrahiert einen Text aus der Dokumentseite mithilfe von Textoptionen (um den Rohtext-Schnellextraktionsmodus zu aktivieren). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | Extrahiert Textbereiche aus dem Dokument. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | Extrahiert Textbereiche aus der Dokumentseite. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | Extrahiert Textbereiche aus dem Dokument mithilfe von Anpassungsoptionen (regulärer Ausdruck, Groß-/Kleinschreibung usw.). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | Extrahiert Textbereiche aus der Dokumentseite mithilfe von Anpassungsoptionen (regulärer Ausdruck, Groß-/Kleinschreibung usw.). |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | Extrahiert ein Inhaltsverzeichnis aus dem Dokument. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate)(Template) | Analysiert das Dokument anhand der vom Benutzer erstellten Vorlage. |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | Analysiert das Dokumentformular. |
| [Search](../../groupdocs.parser/parser/search#search)(string) | Sucht a*keyword* im Dokument. |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | Sucht a*keyword*im Dokument über Suchoptionen (regulärer Ausdruck, Groß-/Kleinschreibung etc.). |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | Gibt die allgemeinen Informationen zu einer Datei zurück. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | Gibt die allgemeinen Informationen zu einer Datei zurück. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | Gibt die allgemeinen Informationen zu einer Datei zurück. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | Gibt die allgemeinen Informationen zu einer Datei zurück. |

### Siehe auch

* namensraum [GroupDocs.Parser](../../groupdocs.parser)
* Montage [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

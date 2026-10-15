---
title: "Parser"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt die Hauptklasse dar, die die Extraktion von Text‑Bild‑Containern und die Parsing‑Funktionalität steuert."
type: docs
weight: 30
url: /de/net/groupdocs.parser/parser/
---

## Parser class

Stellt die Hauptklasse dar, die die Text-, Bild-, Container-Extraktion und Parsing‑Funktionalität steuert.

```csharp
public sealed class Parser : IDisposable
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | Initialisiert eine neue Instanz der [`Parser`](../parser)-Klasse, um Daten aus einer Datenbank zu extrahieren. |
| [Parser](parser#constructor)(EmailConnection) | Initialisiert eine neue Instanz der [`Parser`](../parser)-Klasse, um Daten von einem entfernten E‑Mail‑Server zu extrahieren. |
| [Parser](parser#constructor_4)(Stream) | Initialisiert eine neue Instanz der [`Parser`](../parser)-Klasse. |
| [Parser](parser#constructor_8)(string) | Initialisiert eine neue Instanz der [`Parser`](../parser)-Klasse. |
| [Parser](parser#constructor_12)(Uri) | Initialisiert eine neue Instanz der [`Parser`](../parser)-Klasse, um Daten aus einer URI zu extrahieren. |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | Initialisiert eine neue Instanz der [`Parser`](../parser)-Klasse, um Daten aus einer Datenbank zu extrahieren. |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | Initialisiert eine neue Instanz der [`Parser`](../parser)-Klasse, um Daten von einem entfernten E‑Mail‑Server zu extrahieren. |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | Initialisiert eine neue Instanz der [`Parser`](../parser)-Klasse mit [`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [Parser](parser#constructor_7)(Stream, ParserSettings) | Initialisiert eine neue Instanz der [`Parser`](../parser)-Klasse mit [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_9)(string, LoadOptions) | Initialisiert eine neue Instanz der [`Parser`](../parser)-Klasse mit [`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [Parser](parser#constructor_11)(string, ParserSettings) | Initialisiert eine neue Instanz der [`Parser`](../parser)-Klasse mit [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_13)(Uri, LoadOptions) | Initialisiert eine neue Instanz der [`Parser`](../parser)-Klasse, um Daten aus einer URI mit *loadOptions* zu extrahieren. |
| [Parser](parser#constructor_15)(Uri, ParserSettings) | Initialisiert eine neue Instanz der [`Parser`](../parser)-Klasse, um Daten aus einer URI mit *parserSettings* zu extrahieren. |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | Initialisiert eine neue Instanz der [`Parser`](../parser)-Klasse mit [`LoadOptions`](../../groupdocs.parser.options/loadoptions) und [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_10)(string, LoadOptions, ParserSettings) | Initialisiert eine neue Instanz der [`Parser`](../parser)-Klasse mit [`LoadOptions`](../../groupdocs.parser.options/loadoptions) und [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_14)(Uri, LoadOptions, ParserSettings) | Initialisiert eine neue Instanz der [`Parser`](../parser)-Klasse, um Daten aus einer URI mit *loadOptions* und *parserSettings* zu extrahieren. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | Ruft die unterstützten Funktionen ab. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [GenerateAdjustmentFields](../../groupdocs.parser/parser/generateadjustmentfields)(AdjustmentFieldsOptions) | Erzeugt Felder für die automatische Anpassung von Vorlagenposition und -skalierung. |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | Seitenvorschau abrufen. |
| [GetAnnotations](../../groupdocs.parser/parser/getannotations#getannotations)() | Extrahiert Anmerkungen aus dem Dokument. Hinweis: Derzeit wird nur das PDF‑Format unterstützt. |
| [GetAnnotations](../../groupdocs.parser/parser/getannotations#getannotations_1)(int) | Extrahiert Anmerkungen von der Dokumentenseite. Hinweis: Derzeit wird nur das PDF‑Format unterstützt. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | Extrahiert Barcodes aus dem Dokument. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(BarcodeOptions) | Extrahiert Barcodes aus dem Dokument unter Verwendung von Anpassungsoptionen. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int) | Extrahiert Barcodes von der Dokumentenseite. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_4)(int, BarcodeOptions) | Extrahiert Barcodes von der Dokumentenseite unter Verwendung von Anpassungsoptionen. |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | Extrahiert ein Container‑Objekt aus dem Dokument, um mit Formaten zu arbeiten, die Anhänge, ZIP‑Archive usw. enthalten. |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | Gibt die allgemeinen Informationen zum Dokument zurück. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | Extrahiert einen formatierten Text aus dem Dokument. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | Extrahiert einen formatierten Text aus der Dokumentseite. |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | Extrahiert eine Hervorhebung aus dem Dokument. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | Extrahiert Hyperlinks aus dem Dokument. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | Extrahiert Hyperlinks aus der Dokumentseite. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | Extrahiert Hyperlinks aus dem Dokument mithilfe von Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Hyperlinks enthält). |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | Extrahiert Hyperlinks aus der Dokumentseite mithilfe von Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Hyperlinks enthält). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | Extrahiert Bilder aus dem Dokument. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | Extrahiert Bilder aus der Dokumentseite. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | Extrahiert Bilder aus dem Dokument mithilfe von Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Bilder enthält). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | Extrahiert Bilder aus der Dokumentseite mithilfe von Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Bilder enthält). |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | Extrahiert Metadaten aus dem Dokument. |
| [GetPagePreview](../../groupdocs.parser/parser/getpagepreview#getpagepreview)(int) | Erstellt eine Vorschau der Dokumentseite. |
| [GetPagePreview](../../groupdocs.parser/parser/getpagepreview#getpagepreview_1)(int, PagePreviewOptions) | Erstellt eine Vorschau der Dokumentseite mithilfe von Anpassungsoptionen. |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | Extrahiert einen strukturierten Text aus dem Dokument. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)() | Extrahiert Tabellen aus dem Dokument. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_2)(int) | Extrahiert Tabellen aus der Dokumentseite. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(PageTableAreaOptions) | Extrahiert Tabellen aus dem Dokument. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_3)(int, PageTableAreaOptions) | Extrahiert Tabellen aus der Dokumentseite. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | Extrahiert einen Text aus dem Dokument. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | Extrahiert einen Text aus der Dokumentseite. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | Extrahiert eine Textseite aus dem Dokument mithilfe von Textoptionen (um den Roh‑Schnelltextextraktionsmodus zu aktivieren). |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | Extrahiert einen Text aus der Dokumentseite mithilfe von Textoptionen (um den Roh‑Schnelltextextraktionsmodus zu aktivieren). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | Extrahiert Textbereiche aus dem Dokument. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | Extrahiert Textbereiche aus der Dokumentseite. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | Extrahiert Textbereiche aus dem Dokument mithilfe von Anpassungsoptionen (regulärer Ausdruck, Groß-/Kleinschreibung beachten usw.). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | Extrahiert Textbereiche aus der Dokumentseite mithilfe von Anpassungsoptionen (regulärer Ausdruck, Groß-/Kleinschreibung beachten usw.). |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | Extrahiert ein Inhaltsverzeichnis aus dem Dokument. |
| [GetWorksheetCells](../../groupdocs.parser/parser/getworksheetcells#getworksheetcells)(int) | Extrahiert Arbeitsblattzellen. |
| [GetWorksheetCells](../../groupdocs.parser/parser/getworksheetcells#getworksheetcells_1)(int, WorksheetOptions) | Extrahiert Arbeitsblattzellen mithilfe von Anpassungsoptionen. |
| [GetWorksheetInfo](../../groupdocs.parser/parser/getworksheetinfo#getworksheetinfo_1)() | Extrahiert die Informationen zu allen Arbeitsblättern in der Tabelle. |
| [GetWorksheetInfo](../../groupdocs.parser/parser/getworksheetinfo#getworksheetinfo)(int) | Extrahiert die Informationen zum Arbeitsblatt. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate)(Template) | Parst das Dokument anhand der vom Benutzer erstellten Vorlage. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate_1)(Template, ParseByTemplateOptions) | Parst das Dokument anhand der vom Benutzer erstellten Vorlage unter Verwendung von Anpassungsoptionen. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate_2)(TemplateCollection, ParseByTemplateOptions) | Wählt die am besten geeignete Vorlage aus der bereitgestellten Sammlung aus und parst anschließend das Dokument anhand der ausgewählten Vorlage. |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | Parst das Dokumentformular. |
| [Search](../../groupdocs.parser/parser/search#search)(string) | Durchsucht ein *keyword* im Dokument. |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | Durchsucht ein *keyword* im Dokument unter Verwendung von Suchoptionen (regulärer Ausdruck, Groß-/Kleinschreibung beachten usw.). |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | Gibt die allgemeinen Informationen zu einer Datei zurück. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | Gibt die allgemeinen Informationen zu einer Datei zurück. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | Gibt die allgemeinen Informationen zu einer Datei zurück. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | Gibt die allgemeinen Informationen zu einer Datei zurück. |

### Siehe auch

* namespace [GroupDocs.Parser](../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->

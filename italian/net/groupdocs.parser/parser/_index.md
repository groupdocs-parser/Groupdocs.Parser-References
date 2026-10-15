---
title: "Parser"
second_title: "Riferimento API di GroupDocs.Parser per .NET"
description: "Rappresenta la classe principale che controlla l'estrazione del contenitore di immagini di testo e la funzionalità di parsing."
type: docs
weight: 30
url: /it/net/groupdocs.parser/parser/
---

## Parser class

Rappresenta la classe principale che controlla la funzionalità di estrazione e analisi di testo, immagini e contenitori.

```csharp
public sealed class Parser : IDisposable
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | Inizializza una nuova istanza della classe [`Parser`](../parser) per estrarre dati da un database. |
| [Parser](parser#constructor)(EmailConnection) | Inizializza una nuova istanza della classe [`Parser`](../parser) per estrarre dati da un server di posta elettronica remoto. |
| [Parser](parser#constructor_4)(Stream) | Inizializza una nuova istanza della classe [`Parser`](../parser). |
| [Parser](parser#constructor_8)(string) | Inizializza una nuova istanza della classe [`Parser`](../parser). |
| [Parser](parser#constructor_12)(Uri) | Inizializza una nuova istanza della classe [`Parser`](../parser) per estrarre dati da un URI. |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | Inizializza una nuova istanza della classe [`Parser`](../parser) per estrarre dati da un database. |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | Inizializza una nuova istanza della classe [`Parser`](../parser) per estrarre dati da un server di posta elettronica remoto. |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | Inizializza una nuova istanza della classe [`Parser`](../parser) con [`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [Parser](parser#constructor_7)(Stream, ParserSettings) | Inizializza una nuova istanza della classe [`Parser`](../parser) con [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_9)(string, LoadOptions) | Inizializza una nuova istanza della classe [`Parser`](../parser) con [`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [Parser](parser#constructor_11)(string, ParserSettings) | Inizializza una nuova istanza della classe [`Parser`](../parser) con [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_13)(Uri, LoadOptions) | Inizializza una nuova istanza della classe [`Parser`](../parser) per estrarre dati da un URI con *loadOptions*. |
| [Parser](parser#constructor_15)(Uri, ParserSettings) | Inizializza una nuova istanza della classe [`Parser`](../parser) per estrarre dati da un URI con *parserSettings*. |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | Inizializza una nuova istanza della classe [`Parser`](../parser) con [`LoadOptions`](../../groupdocs.parser.options/loadoptions) e [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_10)(string, LoadOptions, ParserSettings) | Inizializza una nuova istanza della classe [`Parser`](../parser) con [`LoadOptions`](../../groupdocs.parser.options/loadoptions) e [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_14)(Uri, LoadOptions, ParserSettings) | Inizializza una nuova istanza della classe [`Parser`](../parser) per estrarre dati da un URI con *loadOptions* e *parserSettings*. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | Ottiene le funzionalità supportate. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al reset delle risorse non gestite. |
| [GenerateAdjustmentFields](../../groupdocs.parser/parser/generateadjustmentfields)(AdjustmentFieldsOptions) | Genera campi per la regolazione automatica della posizione e della scala del modello. |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | Ottieni l'anteprima delle pagine. |
| [GetAnnotations](../../groupdocs.parser/parser/getannotations#getannotations)() | Estrae le annotazioni dal documento. Nota che attualmente è supportato solo il formato PDF. |
| [GetAnnotations](../../groupdocs.parser/parser/getannotations#getannotations_1)(int) | Estrae le annotazioni dalla pagina del documento. Nota che attualmente è supportato solo il formato PDF. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | Estrae i codici a barre dal documento. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(BarcodeOptions) | Estrae i codici a barre dal documento utilizzando le opzioni di personalizzazione. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int) | Estrae i codici a barre dalla pagina del documento. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_4)(int, BarcodeOptions) | Estrae i codici a barre dalla pagina del documento utilizzando le opzioni di personalizzazione. |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | Estrae un oggetto contenitore dal documento per lavorare con formati che contengono allegati, archivi ZIP ecc. |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | Restituisce le informazioni generali sul documento. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | Estrae un testo formattato dal documento. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | Estrae un testo formattato dalla pagina del documento. |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | Estrae un'evidenziazione dal documento. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | Estrae i collegamenti ipertestuali dal documento. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | Estrae i collegamenti ipertestuali dalla pagina del documento. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | Estrae i collegamenti ipertestuali dal documento utilizzando le opzioni di personalizzazione (per impostare l'area rettangolare che contiene i collegamenti ipertestuali). |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | Estrae i collegamenti ipertestuali dalla pagina del documento utilizzando le opzioni di personalizzazione (per impostare l'area rettangolare che contiene i collegamenti ipertestuali). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | Estrae le immagini dal documento. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | Estrae le immagini dalla pagina del documento. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | Estrae le immagini dal documento utilizzando le opzioni di personalizzazione (per impostare l'area rettangolare che contiene le immagini). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | Estrae le immagini dalla pagina del documento utilizzando le opzioni di personalizzazione (per impostare l'area rettangolare che contiene le immagini). |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | Estrae i metadati dal documento. |
| [GetPagePreview](../../groupdocs.parser/parser/getpagepreview#getpagepreview)(int) | Genera un'anteprima della pagina del documento. |
| [GetPagePreview](../../groupdocs.parser/parser/getpagepreview#getpagepreview_1)(int, PagePreviewOptions) | Genera un'anteprima della pagina del documento utilizzando le opzioni di personalizzazione. |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | Estrae un testo strutturato dal documento. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)() | Estrae le tabelle dal documento. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_2)(int) | Estrae tabelle dalla pagina del documento. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(PageTableAreaOptions) | Estrae le tabelle dal documento. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_3)(int, PageTableAreaOptions) | Estrae tabelle dalla pagina del documento. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | Estrae un testo dal documento. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | Estrae un testo dalla pagina del documento. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | Estrae una pagina di testo dal documento usando le opzioni di testo (per abilitare la modalità di estrazione rapida di testo grezzo). |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | Estrae un testo dalla pagina del documento usando le opzioni di testo (per abilitare la modalità di estrazione rapida di testo grezzo). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | Estrae aree di testo dal documento. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | Estrae aree di testo dalla pagina del documento. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | Estrae aree di testo dal documento usando opzioni di personalizzazione (espressione regolare, distinzione maiuscole/minuscole, ecc.). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | Estrae aree di testo dalla pagina del documento usando opzioni di personalizzazione (espressione regolare, distinzione maiuscole/minuscole, ecc.). |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | Estrae un indice dal documento. |
| [GetWorksheetCells](../../groupdocs.parser/parser/getworksheetcells#getworksheetcells)(int) | Estrae celle del foglio di lavoro. |
| [GetWorksheetCells](../../groupdocs.parser/parser/getworksheetcells#getworksheetcells_1)(int, WorksheetOptions) | Estrae celle del foglio di lavoro usando opzioni di personalizzazione. |
| [GetWorksheetInfo](../../groupdocs.parser/parser/getworksheetinfo#getworksheetinfo_1)() | Estrae le informazioni su tutti i fogli di lavoro nel foglio elettronico. |
| [GetWorksheetInfo](../../groupdocs.parser/parser/getworksheetinfo#getworksheetinfo)(int) | Estrae le informazioni sul foglio di lavoro. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate)(Template) | Analizza il documento con il modello generato dall'utente. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate_1)(Template, ParseByTemplateOptions) | Analizza il documento con il modello generato dall'utente usando opzioni di personalizzazione. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate_2)(TemplateCollection, ParseByTemplateOptions) | Seleziona il modello più adatto dalla collezione fornita e poi analizza il documento rispetto al modello selezionato. |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | Analizza il modulo del documento. |
| [Search](../../groupdocs.parser/parser/search#search)(string) | Cerca una *keyword* nel documento. |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | Cerca una *keyword* nel documento usando opzioni di ricerca (espressione regolare, distinzione maiuscole/minuscole, ecc.). |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | Restituisce le informazioni generali su un file. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | Restituisce le informazioni generali su un file. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | Restituisce le informazioni generali su un file. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | Restituisce le informazioni generali su un file. |

### Vedi anche

* namespace [GroupDocs.Parser](../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

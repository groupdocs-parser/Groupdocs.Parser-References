---
title: Parser
second_title: Riferimento API GroupDocs.Parser per .NET
description: Rappresenta la classe principale che controlla il testo le immagini lestrazione del contenitore e la funzionalità di analisi.
type: docs
weight: 590
url: /it/net/groupdocs.parser/parser/
---
## Parser class

Rappresenta la classe principale che controlla il testo, le immagini, l'estrazione del contenitore e la funzionalità di analisi.

```csharp
public sealed class Parser : IDisposable
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | Inizializza una nuova istanza di[`Parser`](../parser) classe per estrarre i dati da un database. |
| [Parser](parser#constructor)(EmailConnection) | Inizializza una nuova istanza di[`Parser`](../parser) classe per estrarre i dati da un server di posta remoto. |
| [Parser](parser#constructor_4)(Stream) | Inizializza una nuova istanza di[`Parser`](../parser) classe. |
| [Parser](parser#constructor_7)(string) | Inizializza una nuova istanza di[`Parser`](../parser) classe. |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | Inizializza una nuova istanza di[`Parser`](../parser) classe per estrarre i dati da un database. |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | Inizializza una nuova istanza di[`Parser`](../parser) classe per estrarre i dati da un server di posta remoto. |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | Inizializza una nuova istanza di[`Parser`](../parser) classe con[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_8)(string, LoadOptions) | Inizializza una nuova istanza di[`Parser`](../parser) classe con[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | Inizializza una nuova istanza di[`Parser`](../parser) classe con[`LoadOptions`](../../groupdocs.parser.options/loadoptions) e[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_9)(string, LoadOptions, ParserSettings) | Inizializza una nuova istanza di[`Parser`](../parser) classe con[`LoadOptions`](../../groupdocs.parser.options/loadoptions) e[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | Ottiene le funzioni supportate. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | Esegue attività definite dall'applicazione associate alla liberazione, al rilascio o al ripristino di risorse non gestite. |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | Ottieni l'anteprima delle pagine. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | Estrae i codici a barre dal documento. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_2)(int) | Estrae i codici a barre dalla pagina del documento. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(PageAreaOptions) | Estrae i codici a barre dal documento utilizzando le opzioni di personalizzazione (per impostare l'area rettangolare che contiene i codici a barre). |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int, PageAreaOptions) | Estrae i codici a barre dalla pagina del documento utilizzando le opzioni di personalizzazione (per impostare l'area rettangolare che contiene i codici a barre). |
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
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | Estrae un testo strutturato dal documento. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)(PageTableAreaOptions) | Estrae le tabelle dal documento. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(int, PageTableAreaOptions) | Estrae le tabelle dalla pagina del documento. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | Estrae un testo dal documento. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | Estrae un testo dalla pagina del documento. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | Estrae una pagina di testo dal documento utilizzando le opzioni di testo (per abilitare la modalità di estrazione rapida del testo non elaborato). |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | Estrae un testo dalla pagina del documento utilizzando le opzioni di testo (per abilitare la modalità di estrazione rapida del testo non elaborato). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | Estrae aree di testo dal documento. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | Estrae aree di testo dalla pagina del documento. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | Estrae le aree di testo dal documento utilizzando le opzioni di personalizzazione (espressione regolare, match case, ecc.). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | Estrae le aree di testo dalla pagina del documento utilizzando le opzioni di personalizzazione (espressione regolare, match case, ecc.). |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | Estrae un sommario dal documento. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate)(Template) | Analizza il documento in base al modello generato dall'utente. |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | Analizza il modulo del documento. |
| [Search](../../groupdocs.parser/parser/search#search)(string) | Ricerche a*keyword* nel documento. |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | Ricerche a*keyword*nel documento utilizzando le opzioni di ricerca (espressione regolare, match case, ecc.). |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | Restituisce le informazioni generali su un file. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | Restituisce le informazioni generali su un file. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | Restituisce le informazioni generali su un file. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | Restituisce le informazioni generali su un file. |

### Guarda anche

* spazio dei nomi [GroupDocs.Parser](../../groupdocs.parser)
* assemblea [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

---
title: "SearchOptions"
second_title: "Riferimento API di GroupDocs.Parser per .NET"
description: "Inizializza una nuova istanza della classe SearchOptionsgroupdocs.parser.options/searchoptions."
type: docs
weight: 10
url: /it/net/groupdocs.parser.options/searchoptions/searchoptions/
---

## SearchOptions(bool, bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_3}

Inizializza una nuova istanza della classe [`SearchOptions`](../../searchoptions).

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages, HighlightOptions leftHighlightOptions, 
    HighlightOptions rightHighlightOptions)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| matchCase | Boolean | Il valore che indica se il caso del testo non è ignorato. |
| matchWholeWord | Boolean | Il valore che indica se la ricerca di testo è limitata a una parola intera. |
| useRegularExpression | Boolean | Il valore che indica se viene usata un'espressione regolare. |
| searchByPages | Boolean | Il valore che indica se la ricerca viene eseguita per pagine. |
| leftHighlightOptions | HighlightOptions | Le opzioni per l'evidenziazione sinistra. |
| rightHighlightOptions | HighlightOptions | Le opzioni per l'evidenziazione destra. |

### Vedi anche

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, int, HighlightOptions, HighlightOptions) {#constructor_6}

Inizializza una nuova istanza della classe [`SearchOptions`](../../searchoptions) con il limite di pagina.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| matchCase | Boolean | Il valore che indica se il caso del testo non è ignorato. |
| matchWholeWord | Boolean | Il valore che indica se la ricerca di testo è limitata a una parola intera. |
| useRegularExpression | Boolean | Il valore che indica se viene usata un'espressione regolare. |
| maxPageIndex | Int32 | Il valore che indica se la ricerca viene eseguita per pagine. |
| leftHighlightOptions | HighlightOptions | Le opzioni per l'evidenziazione sinistra. |
| rightHighlightOptions | HighlightOptions | Le opzioni per l'evidenziazione destra. |

### Vedi anche

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_5}

Inizializza una nuova istanza della classe [`SearchOptions`](../../searchoptions) che viene utilizzata per la ricerca con le opzioni di evidenziazione per l'estrazione dell'evidenziazione sinistra e destra.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| matchCase | Boolean | Il valore che indica se il caso del testo non è ignorato. |
| matchWholeWord | Boolean | Il valore che indica se la ricerca di testo è limitata a una parola intera. |
| useRegularExpression | Boolean | Il valore che indica se viene usata un'espressione regolare. |
| leftHighlightOptions | HighlightOptions | Le opzioni per l'evidenziazione sinistra. |
| rightHighlightOptions | HighlightOptions | Le opzioni per l'evidenziazione destra. |

### Vedi anche

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions) {#constructor_4}

Inizializza una nuova istanza della classe [`SearchOptions`](../../searchoptions) che viene utilizzata per la ricerca con le stesse opzioni di evidenziazione per l'estrazione dell'evidenziazione sinistra e destra.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions highlightOptions)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| matchCase | Boolean | Il valore che indica se il caso del testo non è ignorato. |
| matchWholeWord | Boolean | Il valore che indica se la ricerca di testo è limitata a una parola intera. |
| useRegularExpression | Boolean | Il valore che indica se viene usata un'espressione regolare. |
| highlightOptions | HighlightOptions | Le opzioni per entrambe le evidenziazioni. |

### Vedi anche

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool) {#constructor_1}

Inizializza una nuova istanza della classe [`SearchOptions`](../../searchoptions) che viene utilizzata per la ricerca senza estrazione dell'evidenziazione.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| matchCase | Boolean | Il valore che indica se il caso del testo non è ignorato. |
| matchWholeWord | Boolean | Il valore che indica se la ricerca di testo è limitata a una parola intera. |
| useRegularExpression | Boolean | Il valore che indica se viene usata un'espressione regolare. |

### Vedi anche

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, bool) {#constructor_2}

Inizializza una nuova istanza della classe [`SearchOptions`](../../searchoptions) che viene utilizzata per la ricerca per pagine e senza estrazione dell'evidenziazione.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| matchCase | Boolean | Il valore che indica se il caso del testo non è ignorato. |
| matchWholeWord | Boolean | Il valore che indica se la ricerca di testo è limitata a una parola intera. |
| useRegularExpression | Boolean | Il valore che indica se viene usata un'espressione regolare. |
| searchByPages | Boolean | Il valore che indica se la ricerca viene eseguita per pagine. |

### Vedi anche

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions() {#constructor}

Inizializza una nuova istanza della classe [`SearchOptions`](../../searchoptions) con valori predefiniti. Vedi le note per i dettagli.

```csharp
public SearchOptions()
```

### Osservazioni

Le seguenti proprietà hanno valori predefiniti:

**[`MatchCase`](../matchcase)**

`false`

**[`MatchWholeWord`](../matchwholeword)**

`false`

**[`UseRegularExpression`](../useregularexpression)**

`false`

**[`LeftHighlightOptions`](../lefthighlightoptions)**

`null`

**[`RightHighlightOptions`](../righthighlightoptions)**

`null`

### Vedi anche

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

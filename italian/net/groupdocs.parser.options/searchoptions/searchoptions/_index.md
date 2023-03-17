---
title: SearchOptions
second_title: Riferimento API GroupDocs.Parser per .NET
description: Inizializza una nuova istanza diSearchOptionsgroupdocs.parser.options/searchoptions classe.
type: docs
weight: 10
url: /it/net/groupdocs.parser.options/searchoptions/searchoptions/
---
## SearchOptions(bool, bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_3}

Inizializza una nuova istanza di[`SearchOptions`](../../searchoptions) classe.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages, HighlightOptions leftHighlightOptions, 
    HighlightOptions rightHighlightOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| matchCase | Boolean | Il valore che indica se un caso di testo non viene ignorato. |
| matchWholeWord | Boolean | Il valore che indica se la ricerca di testo è limitata da una parola intera. |
| useRegularExpression | Boolean | Il valore che indica se viene utilizzata un'espressione regolare. |
| searchByPages | Boolean | Il valore che indica se la ricerca viene eseguita per pagine. |
| leftHighlightOptions | HighlightOptions | Le opzioni per l'evidenziazione a sinistra. |
| rightHighlightOptions | HighlightOptions | Le opzioni per l'evidenziazione giusta. |

### Guarda anche

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* spazio dei nomi [GroupDocs.Parser.Options](../../searchoptions)
* assemblea [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_5}

Inizializza una nuova istanza di[`SearchOptions`](../../searchoptions) classe che viene utilizzata per search con le opzioni di evidenziazione per l'estrazione dell'evidenziazione sinistra e destra.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| matchCase | Boolean | Il valore che indica se un caso di testo non viene ignorato. |
| matchWholeWord | Boolean | Il valore che indica se la ricerca di testo è limitata da una parola intera. |
| useRegularExpression | Boolean | Il valore che indica se viene utilizzata un'espressione regolare. |
| leftHighlightOptions | HighlightOptions | Le opzioni per l'evidenziazione a sinistra. |
| rightHighlightOptions | HighlightOptions | Le opzioni per l'evidenziazione giusta. |

### Guarda anche

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* spazio dei nomi [GroupDocs.Parser.Options](../../searchoptions)
* assemblea [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions) {#constructor_4}

Inizializza una nuova istanza di[`SearchOptions`](../../searchoptions) class che viene utilizzata per search con le stesse opzioni di evidenziazione per l'estrazione dell'evidenziazione sinistra e destra.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions highlightOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| matchCase | Boolean | Il valore che indica se un caso di testo non viene ignorato. |
| matchWholeWord | Boolean | Il valore che indica se la ricerca di testo è limitata da una parola intera. |
| useRegularExpression | Boolean | Il valore che indica se viene utilizzata un'espressione regolare. |
| highlightOptions | HighlightOptions | Le opzioni per entrambi i punti salienti. |

### Guarda anche

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* spazio dei nomi [GroupDocs.Parser.Options](../../searchoptions)
* assemblea [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool) {#constructor_1}

Inizializza una nuova istanza di[`SearchOptions`](../../searchoptions) classe che viene utilizzata per search senza estrazione di evidenziazione.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| matchCase | Boolean | Il valore che indica se un caso di testo non viene ignorato. |
| matchWholeWord | Boolean | Il valore che indica se la ricerca di testo è limitata da una parola intera. |
| useRegularExpression | Boolean | Il valore che indica se viene utilizzata un'espressione regolare. |

### Guarda anche

* class [SearchOptions](../../searchoptions)
* spazio dei nomi [GroupDocs.Parser.Options](../../searchoptions)
* assemblea [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, bool) {#constructor_2}

Inizializza una nuova istanza di[`SearchOptions`](../../searchoptions)classe che viene utilizzata per cercare per pagine e senza estrazione dell'evidenziazione.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| matchCase | Boolean | Il valore che indica se un caso di testo non viene ignorato. |
| matchWholeWord | Boolean | Il valore che indica se la ricerca di testo è limitata da una parola intera. |
| useRegularExpression | Boolean | Il valore che indica se viene utilizzata un'espressione regolare. |
| searchByPages | Boolean | Il valore che indica se la ricerca viene eseguita per pagine. |

### Guarda anche

* class [SearchOptions](../../searchoptions)
* spazio dei nomi [GroupDocs.Parser.Options](../../searchoptions)
* assemblea [GroupDocs.Parser](../../../)

---

## SearchOptions() {#constructor}

Inizializza una nuova istanza di[`SearchOptions`](../../searchoptions) classe con valori predefiniti. Vedere le osservazioni per i dettagli.

```csharp
public SearchOptions()
```

### Osservazioni

Le seguenti proprietà hanno valori predefiniti:

**[`MatchCase`](../matchcase)**

`falso`

**[`MatchWholeWord`](../matchwholeword)**

`falso`

**[`UseRegularExpression`](../useregularexpression)**

`falso`

**[`LeftHighlightOptions`](../lefthighlightoptions)**

`nullo`

**[`RightHighlightOptions`](../righthighlightoptions)**

`nullo`

### Guarda anche

* class [SearchOptions](../../searchoptions)
* spazio dei nomi [GroupDocs.Parser.Options](../../searchoptions)
* assemblea [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

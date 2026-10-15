---
title: "PageTextAreaOptions"
second_title: "Riferimento API di GroupDocs.Parser per .NET"
description: "Inizializza una nuova istanza della classe PageTextAreaOptionsgroupdocs.parser.options/pagetextareaoptions con l'opzione di utilizzo OCR."
type: docs
weight: 10
url: /it/net/groupdocs.parser.options/pagetextareaoptions/pagetextareaoptions/
---

## PageTextAreaOptions() {#constructor}

Inizializza una nuova istanza della classe [`PageTextAreaOptions`](../../pagetextareaoptions) con l'opzione di utilizzo OCR.

```csharp
public PageTextAreaOptions()
```

### Vedi anche

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool) {#constructor_1}

Inizializza una nuova istanza della classe [`PageTextAreaOptions`](../../pagetextareaoptions) con l'opzione di utilizzo OCR.

```csharp
public PageTextAreaOptions(bool useOcr)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| useOcr | Boolean | Il valore che indica se la funzionalità OCR è utilizzata per estrarre le aree di testo. |

### Vedi anche

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool, OcrOptions) {#constructor_2}

Inizializza una nuova istanza della classe [`PageTextAreaOptions`](../../pagetextareaoptions) con la possibilità di impostare le opzioni OCR.

```csharp
public PageTextAreaOptions(bool useOcr, OcrOptions ocrOptions)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| useOcr | Boolean | Il valore che indica se la funzionalità OCR è utilizzata per estrarre le aree di testo. |
| ocrOptions | OcrOptions | Le opzioni aggiuntive per la funzionalità OCR. |

### Vedi anche

* class [OcrOptions](../../ocroptions)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string) {#constructor_3}

Inizializza una nuova istanza della classe [`PageTextAreaOptions`](../../pagetextareaoptions) con l'espressione regolare. Le altre opzioni sono impostate per impostazione predefinita (vedi le note per i dettagli).

```csharp
public PageTextAreaOptions(string expression)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| expression | Stringa | L'espressione regolare. |

### Osservazioni

Le seguenti proprietà hanno valori predefiniti:

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

**[`Rectangle`](../../pageareaoptions/rectangle)**

`null`

### Vedi anche

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle) {#constructor_6}

Inizializza una nuova istanza della classe [`PageTextAreaOptions`](../../pagetextareaoptions) con l'espressione regolare e l'area rettangolare. Le altre opzioni sono impostate per impostazione predefinita (vedi le note per i dettagli).

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| expression | Stringa | L'espressione regolare. |
| rectangle | Rectangle | L'area rettangolare che contiene le aree della pagina. |

### Osservazioni

Le seguenti proprietà hanno valori predefiniti:

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

### Vedi anche

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle, double) {#constructor_7}

Inizializza una nuova istanza della classe [`PageTextAreaOptions`](../../pagetextareaoptions) con l'espressione regolare, l'area rettangolare e la dimensione del bordo ignorato. Le altre opzioni sono impostate per impostazione predefinita (vedi le note per i dettagli).

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle, double rectangleTolerance)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| expression | Stringa | L'espressione regolare. |
| rectangle | Rectangle | L'area rettangolare che contiene le aree della pagina. |
| rectangleTolerance | Double | La dimensione del bordo che viene ignorata quando catturata dall'area rettangolare. È misurata come frazione dell'altezza di un elemento di testo. |

### Vedi anche

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle) {#constructor_4}

Inizializza una nuova istanza della classe [`PageTextAreaOptions`](../../pagetextareaoptions).

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| expression | Stringa | L'espressione regolare. |
| matchCase | Boolean | Il valore che indica se il caso del testo non è ignorato. |
| uniteSegments | Boolean | Il valore che indica se i segmenti sono uniti. |
| ignoreFormatting | Boolean | Il valore che indica se la formattazione del testo è ignorata. |
| rectangle | Rectangle | L'area rettangolare che contiene le aree della pagina. |

### Vedi anche

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle, double) {#constructor_5}

Inizializza una nuova istanza della classe [`PageTextAreaOptions`](../../pagetextareaoptions) con la dimensione del bordo ignorato.

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| expression | Stringa | L'espressione regolare. |
| matchCase | Boolean | Il valore che indica se il caso del testo non è ignorato. |
| uniteSegments | Boolean | Il valore che indica se i segmenti sono uniti. |
| ignoreFormatting | Boolean | Il valore che indica se la formattazione del testo è ignorata. |
| rectangle | Rectangle | L'area rettangolare che contiene le aree della pagina. |
| rectangleTolerance | Double | La dimensione del bordo che viene ignorata quando catturata dall'area rettangolare. È misurata come frazione dell'altezza di un elemento di testo. |

### Vedi anche

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

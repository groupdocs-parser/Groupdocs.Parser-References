---
title: "OcrOptions"
second_title: "Riferimento API di GroupDocs.Parser per .NET"
description: "Inizializza una nuova istanza della classe OcrOptionsgroupdocs.parser.options/ocroptions con area rettangolare."
type: docs
weight: 10
url: /it/net/groupdocs.parser.options/ocroptions/ocroptions/
---

## OcrOptions() {#constructor}

Inizializza una nuova istanza della classe [`OcrOptions`](../../ocroptions) con area rettangolare.

```csharp
public OcrOptions()
```

### Vedi anche

* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(PagePreviewOptions) {#constructor_6}

Inizializza una nuova istanza della classe [`OcrOptions`](../../ocroptions) con area rettangolare.

```csharp
public OcrOptions(PagePreviewOptions pagePreviewOptions)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| pagePreviewOptions | PagePreviewOptions | Un'istanza della classe [`PagePreviewOptions`](../pagepreviewoptions) che imposta le proprietà per la generazione dell'anteprima della pagina del documento. |

### Vedi anche

* class [PagePreviewOptions](../../pagepreviewoptions)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle) {#constructor_1}

Inizializza una nuova istanza della classe [`OcrOptions`](../../ocroptions) con area rettangolare.

```csharp
public OcrOptions(Rectangle rectangle)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| rectangle | Rectangle | L'area rettangolare che limita l'area della pagina utilizzata per il riconoscimento del testo. |

### Vedi anche

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(OcrEventHandler) {#constructor_5}

Inizializza una nuova istanza della classe [`OcrOptions`](../../ocroptions) con l'oggetto [`OcrEventHandler`](../../ocreventhandler).

```csharp
public OcrOptions(OcrEventHandler handler)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| handler | OcrEventHandler | Un'istanza di [`OcrEventHandler`](../../ocreventhandler) per catturare gli eventi OCR. |

### Vedi anche

* class [OcrEventHandler](../../ocreventhandler)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle, OcrEventHandler) {#constructor_2}

Inizializza una nuova istanza della classe [`OcrOptions`](../../ocroptions) con area rettangolare e oggetto [`OcrEventHandler`](../../ocreventhandler).

```csharp
public OcrOptions(Rectangle rectangle, OcrEventHandler handler)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| rectangle | Rectangle | L'area rettangolare che limita l'area della pagina utilizzata per il riconoscimento del testo. |
| handler | OcrEventHandler | Un'istanza di [`OcrEventHandler`](../../ocreventhandler) per catturare gli eventi OCR. |

### Vedi anche

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrEventHandler](../../ocreventhandler)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle, OcrEventHandler, PagePreviewOptions, bool) {#constructor_3}

Inizializza una nuova istanza della classe [`OcrOptions`](../../ocroptions).

```csharp
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, 
    PagePreviewOptions pagePreviewOptions, bool useSpellCheker)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| rectangle | Rectangle | L'area rettangolare che limita l'area della pagina utilizzata per il riconoscimento del testo. |
| handler | OcrEventHandler | Un'istanza di [`OcrEventHandler`](../../ocreventhandler) per catturare gli eventi OCR. |
| pagePreviewOptions | PagePreviewOptions | Un'istanza della classe [`PagePreviewOptions`](../pagepreviewoptions) che imposta le proprietà per la generazione dell'anteprima della pagina del documento. |
| useSpellCheker | Boolean | Il valore che indica se il correttore ortografico è utilizzato. |

### Vedi anche

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrEventHandler](../../ocreventhandler)
* class [PagePreviewOptions](../../pagepreviewoptions)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle, OcrEventHandler, PagePreviewOptions, bool, Language) {#constructor_4}

Inizializza una nuova istanza della classe [`OcrOptions`](../../ocroptions).

```csharp
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, 
    PagePreviewOptions pagePreviewOptions, bool useSpellCheker, Language language)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| rectangle | Rectangle | L'area rettangolare che limita l'area della pagina utilizzata per il riconoscimento del testo. |
| handler | OcrEventHandler | Un'istanza di [`OcrEventHandler`](../../ocreventhandler) per catturare gli eventi OCR. |
| pagePreviewOptions | PagePreviewOptions | Un'istanza della classe [`PagePreviewOptions`](../pagepreviewoptions) che imposta le proprietà per la generazione dell'anteprima della pagina del documento. |
| useSpellCheker | Boolean | Il valore che indica se il correttore ortografico è utilizzato. |
| language | Lingua | La lingua utilizzata per l'OCR. |

### Vedi anche

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrEventHandler](../../ocreventhandler)
* class [PagePreviewOptions](../../pagepreviewoptions)
* enum [Language](../../language)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

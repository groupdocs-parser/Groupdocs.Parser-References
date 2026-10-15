---
title: "OcrOptions"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Initialisiert eine neue Instanz der OcrOptionsgroupdocs.parser.options/ocroptions‑Klasse mit rechteckigem Bereich."
type: docs
weight: 10
url: /de/net/groupdocs.parser.options/ocroptions/ocroptions/
---

## OcrOptions() {#constructor}

Initialisiert eine neue Instanz der [`OcrOptions`](../../ocroptions)-Klasse mit rechteckigem Bereich.

```csharp
public OcrOptions()
```

### Siehe auch

* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(PagePreviewOptions) {#constructor_6}

Initialisiert eine neue Instanz der [`OcrOptions`](../../ocroptions)-Klasse mit rechteckigem Bereich.

```csharp
public OcrOptions(PagePreviewOptions pagePreviewOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pagePreviewOptions | PagePreviewOptions | Eine Instanz der [`PagePreviewOptions`](../pagepreviewoptions)-Klasse, die Eigenschaften für die Generierung der Dokumentseitenvorschau festlegt. |

### Siehe auch

* class [PagePreviewOptions](../../pagepreviewoptions)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle) {#constructor_1}

Initialisiert eine neue Instanz der [`OcrOptions`](../../ocroptions)-Klasse mit rechteckigem Bereich.

```csharp
public OcrOptions(Rectangle rectangle)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Rechteck | Rechteck | Der rechteckige Bereich, der den Seitenbereich einschränkt, der für die Texterkennung verwendet wird. |

### Siehe auch

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(OcrEventHandler) {#constructor_5}

Initialisiert eine neue Instanz der [`OcrOptions`](../../ocroptions)-Klasse mit einem [`OcrEventHandler`](../../ocreventhandler)-Objekt.

```csharp
public OcrOptions(OcrEventHandler handler)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| handler | OcrEventHandler | Eine Instanz von [`OcrEventHandler`](../../ocreventhandler), um OCR‑Ereignisse abzufangen. |

### Siehe auch

* class [OcrEventHandler](../../ocreventhandler)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle, OcrEventHandler) {#constructor_2}

Initialisiert eine neue Instanz der [`OcrOptions`](../../ocroptions)-Klasse mit rechteckigem Bereich und einem [`OcrEventHandler`](../../ocreventhandler)-Objekt.

```csharp
public OcrOptions(Rectangle rectangle, OcrEventHandler handler)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Rechteck | Rechteck | Der rechteckige Bereich, der den Seitenbereich einschränkt, der für die Texterkennung verwendet wird. |
| handler | OcrEventHandler | Eine Instanz von [`OcrEventHandler`](../../ocreventhandler), um OCR‑Ereignisse abzufangen. |

### Siehe auch

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrEventHandler](../../ocreventhandler)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle, OcrEventHandler, PagePreviewOptions, bool) {#constructor_3}

Initialisiert eine neue Instanz der [`OcrOptions`](../../ocroptions)-Klasse.

```csharp
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, 
    PagePreviewOptions pagePreviewOptions, bool useSpellCheker)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Rechteck | Rechteck | Der rechteckige Bereich, der den Seitenbereich einschränkt, der für die Texterkennung verwendet wird. |
| handler | OcrEventHandler | Eine Instanz von [`OcrEventHandler`](../../ocreventhandler), um OCR‑Ereignisse abzufangen. |
| pagePreviewOptions | PagePreviewOptions | Eine Instanz der [`PagePreviewOptions`](../pagepreviewoptions)-Klasse, die Eigenschaften für die Generierung der Dokumentseitenvorschau festlegt. |
| useSpellCheker | Boolean | Der Wert, der angibt, ob die Rechtschreibprüfung verwendet wird. |

### Siehe auch

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrEventHandler](../../ocreventhandler)
* class [PagePreviewOptions](../../pagepreviewoptions)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle, OcrEventHandler, PagePreviewOptions, bool, Language) {#constructor_4}

Initialisiert eine neue Instanz der [`OcrOptions`](../../ocroptions)-Klasse.

```csharp
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, 
    PagePreviewOptions pagePreviewOptions, bool useSpellCheker, Language language)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Rechteck | Rechteck | Der rechteckige Bereich, der den Seitenbereich einschränkt, der für die Texterkennung verwendet wird. |
| handler | OcrEventHandler | Eine Instanz von [`OcrEventHandler`](../../ocreventhandler), um OCR‑Ereignisse abzufangen. |
| pagePreviewOptions | PagePreviewOptions | Eine Instanz der [`PagePreviewOptions`](../pagepreviewoptions)-Klasse, die Eigenschaften für die Generierung der Dokumentseitenvorschau festlegt. |
| useSpellCheker | Boolean | Der Wert, der angibt, ob die Rechtschreibprüfung verwendet wird. |
| language | Sprache | Die für OCR verwendete Sprache. |

### Siehe auch

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrEventHandler](../../ocreventhandler)
* class [PagePreviewOptions](../../pagepreviewoptions)
* enum [Language](../../language)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->

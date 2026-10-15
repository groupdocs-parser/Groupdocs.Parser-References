---
title: "OcrOptions"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt die Optionen bereit, die für den OCR‑Connector verwendet werden."
type: docs
weight: 450
url: /de/net/groupdocs.parser.options/ocroptions/
---

## OcrOptions class

Stellt die Optionen bereit, die für den OCR‑Connector verwendet werden.

```csharp
public class OcrOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [OcrOptions](ocroptions#constructor)() | Initialisiert eine neue Instanz der [`OcrOptions`](../ocroptions)-Klasse mit rechteckigem Bereich. |
| [OcrOptions](ocroptions#constructor_5)(OcrEventHandler) | Initialisiert eine neue Instanz der [`OcrOptions`](../ocroptions)-Klasse mit dem [`OcrEventHandler`](../ocreventhandler)-Objekt. |
| [OcrOptions](ocroptions#constructor_6)(PagePreviewOptions) | Initialisiert eine neue Instanz der [`OcrOptions`](../ocroptions)-Klasse mit rechteckigem Bereich. |
| [OcrOptions](ocroptions#constructor_1)(Rectangle) | Initialisiert eine neue Instanz der [`OcrOptions`](../ocroptions)-Klasse mit rechteckigem Bereich. |
| [OcrOptions](ocroptions#constructor_2)(Rectangle, OcrEventHandler) | Initialisiert eine neue Instanz der [`OcrOptions`](../ocroptions)-Klasse mit rechteckigem Bereich und dem [`OcrEventHandler`](../ocreventhandler)-Objekt. |
| [OcrOptions](ocroptions#constructor_3)(Rectangle, OcrEventHandler, PagePreviewOptions, bool) | Initialisiert eine neue Instanz der [`OcrOptions`](../ocroptions)-Klasse. |
| [OcrOptions](ocroptions#constructor_4)(Rectangle, OcrEventHandler, PagePreviewOptions, bool, Language) | Initialisiert eine neue Instanz der [`OcrOptions`](../ocroptions)-Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Handler](../../groupdocs.parser.options/ocroptions/handler) { get; set; } | Liefert den Ereignishandler, um OCR-Ereignisse abzufangen. |
| [Language](../../groupdocs.parser.options/ocroptions/language) { get; set; } | Liest oder setzt die für OCR verwendete Sprache. Bestimmt das bei der Erkennung verwendete Alphabet. Englisch wird standardmäßig verwendet. |
| [PagePreviewOptions](../../groupdocs.parser.options/ocroptions/pagepreviewoptions) { get; set; } | Liest die Optionen für die Dokumentseitenvorschau. |
| [Rectangle](../../groupdocs.parser.options/ocroptions/rectangle) { get; set; } | Liest den rechteckigen Bereich, der den Seitenbereich einschränkt, der für die Texterkennung verwendet wird. |
| [UseSpellChecker](../../groupdocs.parser.options/ocroptions/usespellchecker) { get; set; } | Liest den Wert, der angibt, ob die Rechtschreibprüfung verwendet wird. |

### Siehe auch

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->

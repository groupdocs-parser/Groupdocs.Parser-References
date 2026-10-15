---
title: "RecognizeTextAreas"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Erkenne Textbereiche aus dem imageStream-Stream."
type: docs
weight: 40
url: /de/net/groupdocs.parser.options/ocrconnectorbase/recognizetextareas/
---

## RecognizeTextAreas(Stream, Page, OcrOptions) {#recognizetextareas}

Erkenne Textbereiche aus dem *imageStream*-Stream.

```csharp
public virtual IList<PageTextArea> RecognizeTextAreas(Stream imageStream, Page page, 
    OcrOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| imageStream | Stream | Die Bilddarstellung der Dokumentenseite. |
| Seite | Page | Die die Dokumentenseite. |
| options | OcrOptions | Die OCR-Optionen. |

### Rückgabewert

Eine Sammlung von [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea)-Objekten; `null`, wenn die Erkennung von Textbereichen nicht unterstützt wird.

### Siehe auch

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Page](../../../groupdocs.parser.data/page)
* class [OcrOptions](../../ocroptions)
* class [OcrConnectorBase](../../ocrconnectorbase)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## RecognizeTextAreas(Stream, IEnumerable&lt;Rectangle&gt;, string, Page, OcrOptions) {#recognizetextareas_3}

Erkenne Textbereiche aus dem *imageStream*-Stream.

```csharp
public virtual IList<PageTextArea> RecognizeTextAreas(Stream imageStream, 
    IEnumerable<Rectangle> rectangles, string allowedSymbols, Page page, OcrOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| imageStream | Stream | Die Bilddarstellung der Dokumentenseite. |
| rectangles | IEnumerable`1 | Die Sammlung rechteckiger Bereiche, die die OCR-Funktionalität einschränkt. |
| allowedSymbols | String | Der Filter zulässiger Symbole durch OCR. |
| Seite | Page | Die die Dokumentenseite. |
| options | OcrOptions | Die OCR-Optionen. |

### Rückgabewert

Eine Sammlung von [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea)-Objekten; `null`, wenn die Erkennung von Textbereichen nicht unterstützt wird.

### Siehe auch

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [Page](../../../groupdocs.parser.data/page)
* class [OcrOptions](../../ocroptions)
* class [OcrConnectorBase](../../ocrconnectorbase)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->

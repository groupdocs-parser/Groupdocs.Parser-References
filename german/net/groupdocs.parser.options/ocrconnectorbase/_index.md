---
title: "OcrConnectorBase"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt die OCR‑Funktionalität bereit."
type: docs
weight: 430
url: /de/net/groupdocs.parser.options/ocrconnectorbase/
---

## OcrConnectorBase class

Stellt die OCR‑Funktionalität bereit.

```csharp
public abstract class OcrConnectorBase
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| virtual [IsTextAreasSupported](../../groupdocs.parser.options/ocrconnectorbase/istextareassupported) { get; } | Gibt den Wert zurück, der angibt, ob die Extraktion von Textbereichen unterstützt wird. |
| virtual [IsTextSupported](../../groupdocs.parser.options/ocrconnectorbase/istextsupported) { get; } | Gibt den Wert zurück, der angibt, ob die Textextraktion unterstützt wird. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| virtual [RecognizeText](../../groupdocs.parser.options/ocrconnectorbase/recognizetext#recognizetext)(Stream, OcrOptions) | Erkenne einen Text aus dem *imageStream*-Stream. |
| virtual [RecognizeTextAreas](../../groupdocs.parser.options/ocrconnectorbase/recognizetextareas#recognizetextareas)(Stream, Page, OcrOptions) | Erkenne Textbereiche aus dem *imageStream*-Stream. |
| virtual [RecognizeTextAreas](../../groupdocs.parser.options/ocrconnectorbase/recognizetextareas#recognizetextareas_3)(Stream, IEnumerable&lt;Rectangle&gt;, string, Page, OcrOptions) | Erkenne Textbereiche aus dem *imageStream*-Stream. |

### Siehe auch

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->

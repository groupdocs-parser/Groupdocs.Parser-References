---
title: "BarcodeOptions"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt die Optionen bereit, die für die Barcode-Extraktion verwendet werden."
type: docs
weight: 200
url: /de/net/groupdocs.parser.options/barcodeoptions/
---

## BarcodeOptions class

Stellt die Optionen bereit, die für die Barcode-Extraktion verwendet werden.

```csharp
public sealed class BarcodeOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [BarcodeOptions](barcodeoptions#constructor)() | Initialisiert eine neue Instanz der Klasse [`BarcodeOptions`](../barcodeoptions) mit Standardwerten. |
| [BarcodeOptions](barcodeoptions#constructor_1)(Rectangle) | Initialisiert eine neue Instanz der Klasse [`BarcodeOptions`](../barcodeoptions) mit dem rechteckigen Bereich. |
| [BarcodeOptions](barcodeoptions#constructor_3)(QualityMode, QualityMode, params string[]) | Initialisiert eine neue Instanz der Klasse [`BarcodeOptions`](../barcodeoptions) mit Qualitätseinstellungen und Code‑Typen. |
| [BarcodeOptions](barcodeoptions#constructor_2)(Rectangle, QualityMode, QualityMode, float?, bool, params string[]) | Initialisiert eine neue Instanz der Klasse [`BarcodeOptions`](../barcodeoptions). |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AllowIncorrectBarcodes](../../groupdocs.parser.options/barcodeoptions/allowincorrectbarcodes) { get; set; } | Ruft den Wert ab, der angibt, ob fehlerhafte Barcodes erlaubt sind. |
| [BarcodeQuality](../../groupdocs.parser.options/barcodeoptions/barcodequality) { get; set; } | Ruft die Qualität eines Quell‑Barcodes ab. |
| [CodeTypes](../../groupdocs.parser.options/barcodeoptions/codetypes) { get; set; } | Ruft die zu lesenden Barcode‑Typen ab. |
| [Dimension](../../groupdocs.parser.options/barcodeoptions/dimension) { get; set; } | Ruft die minimale Größe des kleinsten Barcode‑Elements ab. |
| [ImageQuality](../../groupdocs.parser.options/barcodeoptions/imagequality) { get; set; } | Ruft die Qualität eines Quell‑Bildes ab. |
| [PagePreviewOptions](../../groupdocs.parser.options/barcodeoptions/pagepreviewoptions) { get; set; } | Ruft die Vorschaueinstellungen der Dokumentenseite ab oder legt sie fest. |
| [Rectangle](../../groupdocs.parser.options/barcodeoptions/rectangle) { get; set; } | Liest den rechteckigen Bereich, der Seitenbereiche enthält. |

### Siehe auch

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->

---
title: "BarcodeOptions"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Initialisiert eine neue Instanz der BarcodeOptionsgroupdocs.parser.options/barcodeoptions-Klasse mit Standardwerten."
type: docs
weight: 10
url: /de/net/groupdocs.parser.options/barcodeoptions/barcodeoptions/
---

## BarcodeOptions() {#constructor}

Initialisiert eine neue Instanz der [`BarcodeOptions`](../../barcodeoptions)-Klasse mit Standardwerten.

```csharp
public BarcodeOptions()
```

### Siehe auch

* class [BarcodeOptions](../../barcodeoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## BarcodeOptions(Rectangle) {#constructor_1}

Initialisiert eine neue Instanz der [`BarcodeOptions`](../../barcodeoptions)-Klasse mit dem rechteckigen Bereich.

```csharp
public BarcodeOptions(Rectangle rectangle)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Rechteck | Rechteck | Der rechteckige Bereich, der Barcodes enthält. |

### Siehe auch

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [BarcodeOptions](../../barcodeoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## BarcodeOptions(QualityMode, QualityMode, params string[]) {#constructor_3}

Initialisiert eine neue Instanz der [`BarcodeOptions`](../../barcodeoptions)-Klasse mit Qualitätseinstellungen und Code-Typen.

```csharp
public BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, 
    params string[] codeTypes)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| imageQuality | QualityMode | Die Qualität eines Quellbildes. |
| barcodeQuality | QualityMode | Die Qualität eines Quell-Barcodes. |
| codeTypes | String[] | Die Typen von Barcodes, die gelesen werden sollen. |

### Siehe auch

* enum [QualityMode](../../qualitymode)
* class [BarcodeOptions](../../barcodeoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## BarcodeOptions(Rectangle, QualityMode, QualityMode, float?, bool, params string[]) {#constructor_2}

Initialisiert eine neue Instanz der [`BarcodeOptions`](../../barcodeoptions)-Klasse.

```csharp
public BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, 
    float? dimension, bool allowIncorrectBarcodes, params string[] codeTypes)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Rechteck | Rechteck | Der rechteckige Bereich, der Barcodes enthält. |
| imageQuality | QualityMode | Die Qualität eines Quellbildes. |
| barcodeQuality | QualityMode | Die Qualität eines Quell-Barcodes. |
| Dimension | Nullable`1 | Die minimale Größe des minimalen Barcode-Elements. |
| allowIncorrectBarcodes | Boolean | Der Wert, der angibt, ob falsche Barcodes erlaubt sind. |
| codeTypes | String[] | Die Typen von Barcodes, die gelesen werden sollen. |

### Siehe auch

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* enum [QualityMode](../../qualitymode)
* class [BarcodeOptions](../../barcodeoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->

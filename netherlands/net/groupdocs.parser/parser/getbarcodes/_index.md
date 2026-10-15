---
title: "GetBarcodes"
second_title: "GroupDocs.Parser voor .NET API-referentie"
description: "Extraheert barcodes uit het document."
type: docs
weight: 70
url: /nl/net/groupdocs.parser/parser/getbarcodes/
---

## GetBarcodes() {#getbarcodes}

Extraheert barcodes uit het document.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes()
```

### Retourwaarde

Een verzameling van [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objecten; `null` als barcode‑extractie niet wordt ondersteund.

### Voorbeelden

Het volgende voorbeeld toont hoe barcodes uit een document te extraheren:

```csharp
// Maak een instantie van de Parser‑klasse
using (Parser parser = new Parser(filePath))
{
    // Extraheer barcodes uit het document.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes();

    // Itereer over barcodes
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Print de paginanaanduiding
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Print de barcode-waarde
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Zie ook

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(int) {#getbarcodes_3}

Extraheert barcodes van de documentpagina.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageIndex | Int32 | De nulgebaseerde paginapositie. |

### Retourwaarde

Een verzameling van [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objecten; `null` als barcode‑extractie niet wordt ondersteund.

### Voorbeelden

Het volgende voorbeeld toont hoe barcodes uit een documentpagina te extraheren:

```csharp
// Maak een instantie van de Parser‑klasse
using (Parser parser = new Parser(filePath))
{
    // Extraheer barcodes uit de tweede documentpagina.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(1);

    // Itereer over barcodes
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Print de paginanaanduiding
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Print de barcode-waarde
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Zie ook

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(BarcodeOptions) {#getbarcodes_1}

Extraheert barcodes uit het document met behulp van aanpassingsopties.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(BarcodeOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| options | BarcodeOptions | De opties voor het extraheren van barcodes. |

### Retourwaarde

Een verzameling van [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objecten; `null` als barcode‑extractie niet wordt ondersteund.

### Voorbeelden

Het volgende voorbeeld toont hoe barcodes uit de rechterbovenhoek te extraheren.

```csharp
// Maak een instantie van de Parser‑klasse
using (Parser parser = new Parser(filePath))
{
    // Maak de opties die worden gebruikt voor het extraheren van barcodes
    BarcodeOptions options = new BarcodeOptions(new Rectangle(new Point(590, 80), new Size(150, 150)));
    // Extraheer barcodes uit de rechterbovenhoek.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(options);

    // Itereer over barcodes
    foreach (PageBarcodeArea barcode in barcodes)
    {
        // Print de paginanaanduiding
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Print de barcode-waarde
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Zie ook

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [BarcodeOptions](../../../groupdocs.parser.options/barcodeoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(int, BarcodeOptions) {#getbarcodes_4}

Extraheert barcodes van de documentpagina met behulp van aanpassingsopties.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex, BarcodeOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageIndex | Int32 | De nulgebaseerde paginapositie. |
| options | BarcodeOptions | De opties voor het extraheren van barcodes. |

### Retourwaarde

Een verzameling van [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objecten; `null` als barcode‑extractie niet wordt ondersteund.

### Zie ook

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [BarcodeOptions](../../../groupdocs.parser.options/barcodeoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

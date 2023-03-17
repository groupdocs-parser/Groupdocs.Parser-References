---
title: GetBarcodes
second_title: GroupDocs.Parser voor .NET API-referentie
description: Haalt streepjescodes uit het document.
type: docs
weight: 50
url: /nl/net/groupdocs.parser/parser/getbarcodes/
---
## GetBarcodes() {#getbarcodes}

Haalt streepjescodes uit het document.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes()
```

### Winstwaarde

Een verzameling van[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objecten; `nul` als extractie van streepjescodes niet wordt ondersteund.

### Voorbeelden

Het volgende voorbeeld laat zien hoe streepjescodes uit een document gehaald kunnen worden:

```csharp
// Maak een instantie van de Parser-klasse
using (Parser parser = new Parser(filePath))
{
    // Extraheer streepjescodes uit het document.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes();

    // Itereren over streepjescodes
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Druk de pagina-index af
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Druk de streepjescodewaarde af
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Zie ook

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## GetBarcodes(int) {#getbarcodes_2}

Haalt streepjescodes uit de documentpagina.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageIndex | Int32 | De op nul gebaseerde pagina-index. |

### Winstwaarde

Een verzameling van[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objecten; `nul` als extractie van streepjescodes niet wordt ondersteund.

### Voorbeelden

Het volgende voorbeeld laat zien hoe streepjescodes uit een documentpagina gehaald kunnen worden:

```csharp
// Maak een instantie van de Parser-klasse
using (Parser parser = new Parser(filePath))
{
    // Extraheer streepjescodes van de tweede documentpagina.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(1);

    // Itereren over streepjescodes
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Druk de pagina-index af
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Druk de streepjescodewaarde af
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Zie ook

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## GetBarcodes(PageAreaOptions) {#getbarcodes_1}

Haalt streepjescodes uit het document met behulp van aanpassingsopties (om het rechthoekige gebied in te stellen dat streepjescodes bevat).

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(PageAreaOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| options | PageAreaOptions | De opties voor extractie van streepjescodes. |

### Winstwaarde

Een verzameling van[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objecten; `nul` als extractie van streepjescodes niet wordt ondersteund.

### Voorbeelden

Het volgende voorbeeld laat zien hoe streepjescodes uit de rechterbovenhoek kunnen worden geëxtraheerd.

```csharp
// Maak een instantie van de Parser-klasse
using (Parser parser = new Parser(filePath))
{
    // Creëer de opties die worden gebruikt voor het extraheren van streepjescodes
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(590, 80), new Size(150, 150)));
    // Pak streepjescodes uit de rechterbovenhoek.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(options);

    // Itereren over streepjescodes
    foreach (PageBarcodeArea barcode in barcodes)
    {
        // Druk de pagina-index af
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Druk de streepjescodewaarde af
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Zie ook

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## GetBarcodes(int, PageAreaOptions) {#getbarcodes_3}

Haalt streepjescodes uit de documentpagina met behulp van aanpassingsopties (om het rechthoekige gebied in te stellen dat streepjescodes bevat).

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex, PageAreaOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageIndex | Int32 | De op nul gebaseerde pagina-index. |
| options | PageAreaOptions | De opties voor extractie van streepjescodes. |

### Winstwaarde

Een verzameling van[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objecten; `nul` als extractie van streepjescodes niet wordt ondersteund.

### Zie ook

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

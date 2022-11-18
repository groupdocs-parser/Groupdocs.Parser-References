---
title: GetBarcodes
second_title: GroupDocs.Parser för .NET API-referens
description: Extraherar streckkoder från dokumentet.
type: docs
weight: 50
url: /sv/net/groupdocs.parser/parser/getbarcodes/
---
## GetBarcodes() {#getbarcodes}

Extraherar streckkoder från dokumentet.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes()
```

### Returvärde

En samling av[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objekt; `null` om extrahering av streckkoder inte stöds.

### Exempel

Följande exempel visar hur man extraherar streckkoder från ett dokument:

```csharp
// Skapa en instans av Parser-klassen
using (Parser parser = new Parser(filePath))
{
    // Extrahera streckkoder från dokumentet.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes();

    // Iterera över streckkoder
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Skriv ut sidindexet
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Skriv ut streckkodsvärdet
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Se även

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## GetBarcodes(int) {#getbarcodes_2}

Extraherar streckkoder från dokumentsidan.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | Det nollbaserade sidindexet. |

### Returvärde

En samling av[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objekt; `null` om extrahering av streckkoder inte stöds.

### Exempel

Följande exempel visar hur man extraherar streckkoder från en dokumentsida:

```csharp
// Skapa en instans av Parser-klassen
using (Parser parser = new Parser(filePath))
{
    // Extrahera streckkoder från den andra dokumentsidan.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(1);

    // Iterera över streckkoder
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Skriv ut sidindexet
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Skriv ut streckkodsvärdet
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Se även

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## GetBarcodes(PageAreaOptions) {#getbarcodes_1}

Extraherar streckkoder från dokumentet med hjälp av anpassningsalternativ (för att ställa in det rektangulära område som innehåller streckkoder).

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(PageAreaOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| options | PageAreaOptions | Alternativen för extrahering av streckkoder. |

### Returvärde

En samling av[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objekt; `null` om extrahering av streckkoder inte stöds.

### Exempel

Följande exempel visar hur man extraherar streckkoder från det övre högra hörnet.

```csharp
// Skapa en instans av Parser-klassen
using (Parser parser = new Parser(filePath))
{
    // Skapa alternativen som används för att extrahera streckkoder
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(590, 80), new Size(150, 150)));
    // Extrahera streckkoder från det övre högra hörnet.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(options);

    // Iterera över streckkoder
    foreach (PageBarcodeArea barcode in barcodes)
    {
        // Skriv ut sidindexet
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Skriv ut streckkodsvärdet
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Se även

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## GetBarcodes(int, PageAreaOptions) {#getbarcodes_3}

Extraherar streckkoder från dokumentsidan med hjälp av anpassningsalternativ (för att ställa in det rektangulära område som innehåller streckkoder).

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex, PageAreaOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | Det nollbaserade sidindexet. |
| options | PageAreaOptions | Alternativen för extrahering av streckkoder. |

### Returvärde

En samling av[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objekt; `null` om extrahering av streckkoder inte stöds.

### Se även

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

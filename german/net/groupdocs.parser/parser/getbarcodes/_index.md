---
title: GetBarcodes
second_title: GroupDocs.Parser für .NET-API-Referenz
description: Extrahiert Barcodes aus dem Dokument.
type: docs
weight: 50
url: /de/net/groupdocs.parser/parser/getbarcodes/
---
## GetBarcodes() {#getbarcodes}

Extrahiert Barcodes aus dem Dokument.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes()
```

### Rückgabewert

Eine Sammlung von[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) Objekte; `Null` wenn die Barcode-Extraktion nicht unterstützt wird.

### Beispiele

Das folgende Beispiel zeigt, wie Barcodes aus einem Dokument extrahiert werden:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse
using (Parser parser = new Parser(filePath))
{
    // Barcodes aus dem Dokument extrahieren.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes();

    // Strichcodes durchlaufen
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Den Seitenindex drucken
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Barcodewert drucken
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Siehe auch

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## GetBarcodes(int) {#getbarcodes_2}

Extrahiert Barcodes von der Dokumentseite.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | Int32 | Der nullbasierte Seitenindex. |

### Rückgabewert

Eine Sammlung von[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) Objekte; `Null` wenn die Barcode-Extraktion nicht unterstützt wird.

### Beispiele

Das folgende Beispiel zeigt, wie Barcodes aus einer Dokumentseite extrahiert werden:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse
using (Parser parser = new Parser(filePath))
{
    // Barcodes von der zweiten Dokumentseite extrahieren.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(1);

    // Strichcodes durchlaufen
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Den Seitenindex drucken
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Barcodewert drucken
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Siehe auch

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## GetBarcodes(PageAreaOptions) {#getbarcodes_1}

Extrahiert Barcodes aus dem Dokument mithilfe der Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Barcodes enthält).

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(PageAreaOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | PageAreaOptions | Die Optionen für die Barcode-Extraktion. |

### Rückgabewert

Eine Sammlung von[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) Objekte; `Null` wenn die Barcode-Extraktion nicht unterstützt wird.

### Beispiele

Das folgende Beispiel zeigt, wie Barcodes aus der oberen rechten Ecke extrahiert werden.

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse
using (Parser parser = new Parser(filePath))
{
    // Erstellen Sie die Optionen, die für die Barcode-Extraktion verwendet werden
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(590, 80), new Size(150, 150)));
    // Barcodes aus der oberen rechten Ecke extrahieren.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(options);

    // Strichcodes durchlaufen
    foreach (PageBarcodeArea barcode in barcodes)
    {
        // Den Seitenindex drucken
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Barcodewert drucken
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Siehe auch

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## GetBarcodes(int, PageAreaOptions) {#getbarcodes_3}

Extrahiert Barcodes von der Dokumentseite mithilfe von Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Barcodes enthält).

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex, PageAreaOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | Int32 | Der nullbasierte Seitenindex. |
| options | PageAreaOptions | Die Optionen für die Barcode-Extraktion. |

### Rückgabewert

Eine Sammlung von[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) Objekte; `Null` wenn die Barcode-Extraktion nicht unterstützt wird.

### Siehe auch

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

---
title: "GetBarcodes"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Extrahiert Barcodes aus dem Dokument."
type: docs
weight: 70
url: /de/net/groupdocs.parser/parser/getbarcodes/
---

## GetBarcodes() {#getbarcodes}

Extrahiert Barcodes aus dem Dokument.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes()
```

### Rückgabewert

Eine Sammlung von [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea)-Objekten; `null`, wenn die Barcode-Extraktion nicht unterstützt wird.

### Beispiele

Das folgende Beispiel zeigt, wie Barcodes aus einem Dokument extrahiert werden:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using (Parser parser = new Parser(filePath))
{
    // Barcodes aus dem Dokument extrahieren.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes();

    // Iterieren Sie über Barcodes
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Geben Sie den Seitenindex aus
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Geben Sie den Barcode-Wert aus
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Siehe auch

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(int) {#getbarcodes_3}

Extrahiert Barcodes von der Dokumentenseite.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | Int32 | Der nullbasierte Seitenindex. |

### Rückgabewert

Eine Sammlung von [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea)-Objekten; `null`, wenn die Barcode-Extraktion nicht unterstützt wird.

### Beispiele

Das folgende Beispiel zeigt, wie Barcodes aus einer Dokumentenseite extrahiert werden:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using (Parser parser = new Parser(filePath))
{
    // Barcodes aus der zweiten Dokumentenseite extrahieren.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(1);

    // Iterieren Sie über Barcodes
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Geben Sie den Seitenindex aus
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Geben Sie den Barcode-Wert aus
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Siehe auch

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(BarcodeOptions) {#getbarcodes_1}

Extrahiert Barcodes aus dem Dokument unter Verwendung von Anpassungsoptionen.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(BarcodeOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | BarcodeOptions | Die Optionen für die Barcode-Extraktion. |

### Rückgabewert

Eine Sammlung von [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea)-Objekten; `null`, wenn die Barcode-Extraktion nicht unterstützt wird.

### Beispiele

Das folgende Beispiel zeigt, wie man Barcodes aus der oberen rechten Ecke extrahiert.

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using (Parser parser = new Parser(filePath))
{
    // Erstellen Sie die Optionen, die für die Barcode-Extraktion verwendet werden
    BarcodeOptions options = new BarcodeOptions(new Rectangle(new Point(590, 80), new Size(150, 150)));
    // Extrahieren Sie Barcodes aus der oberen rechten Ecke.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(options);

    // Iterieren Sie über Barcodes
    foreach (PageBarcodeArea barcode in barcodes)
    {
        // Geben Sie den Seitenindex aus
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Geben Sie den Barcode-Wert aus
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Siehe auch

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [BarcodeOptions](../../../groupdocs.parser.options/barcodeoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(int, BarcodeOptions) {#getbarcodes_4}

Extrahiert Barcodes von der Dokumentenseite unter Verwendung von Anpassungsoptionen.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex, BarcodeOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | Int32 | Der nullbasierte Seitenindex. |
| options | BarcodeOptions | Die Optionen für die Barcode-Extraktion. |

### Rückgabewert

Eine Sammlung von [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea)-Objekten; `null`, wenn die Barcode-Extraktion nicht unterstützt wird.

### Siehe auch

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [BarcodeOptions](../../../groupdocs.parser.options/barcodeoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->

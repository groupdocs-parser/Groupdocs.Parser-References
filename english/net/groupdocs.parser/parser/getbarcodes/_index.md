---
title: GetBarcodes
second_title: GroupDocs.Parser for .NET API Reference
description: Extracts barcodes from the document.
type: docs
weight: 50
url: /net/groupdocs.parser/parser/getbarcodes/
---
## GetBarcodes() {#getbarcodes}

Extracts barcodes from the document.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes()
```

### Return Value

A collection of [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objects; `null` if barcodes extraction isn't supported.

### Examples

The following example shows how to extract barcodes from a document:

```csharp
// Create an instance of Parser class
using (Parser parser = new Parser(filePath))
{
    // Extract barcodes from the document.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes();

    // Iterate over barcodes
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Print the page index
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Print the barcode value
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### See Also

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(int) {#getbarcodes_2}

Extracts barcodes from the document page.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | The zero-based page index. |

### Return Value

A collection of [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objects; `null` if barcodes extraction isn't supported.

### Examples

The following example shows how to extract barcodes from a document page:

```csharp
// Create an instance of Parser class
using (Parser parser = new Parser(filePath))
{
    // Extract barcodes from the second document page.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(1);

    // Iterate over barcodes
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Print the page index
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Print the barcode value
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### See Also

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(PageAreaOptions) {#getbarcodes_1}

Extracts barcodes from the document using customization options (to set the rectangular area that contains barcodes).

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(PageAreaOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| options | PageAreaOptions | The options for barcodes extraction. |

### Return Value

A collection of [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objects; `null` if barcodes extraction isn't supported.

### Examples

The following example shows how to extract barcodes from the upper-right corner.

```csharp
// Create an instance of Parser class
using (Parser parser = new Parser(filePath))
{
    // Create the options which are used for barcodes extraction
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(590, 80), new Size(150, 150)));
    // Extract barcodes from the upper-right corner.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(options);

    // Iterate over barcodes
    foreach (PageBarcodeArea barcode in barcodes)
    {
        // Print the page index
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Print the barcode value
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### See Also

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(int, PageAreaOptions) {#getbarcodes_3}

Extracts barcodes from the document page using customization options (to set the rectangular area that contains barcodes).

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex, PageAreaOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | The zero-based page index. |
| options | PageAreaOptions | The options for barcodes extraction. |

### Return Value

A collection of [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objects; `null` if barcodes extraction isn't supported.

### See Also

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.parser.dll -->

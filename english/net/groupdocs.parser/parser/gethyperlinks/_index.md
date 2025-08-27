---
title: GetHyperlinks
second_title: GroupDocs.Parser for .NET API Reference
description: Extracts hyperlinks from the document.
type: docs
weight: 110
url: /net/groupdocs.parser/parser/gethyperlinks/
---
## GetHyperlinks() {#gethyperlinks}

Extracts hyperlinks from the document.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks()
```

### Return Value

A collection of [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objects; `null` if hyperlinks extraction isn't supported.

### Examples

The following example shows how to extract all hyperlinks from the whole document:

```csharp
// Create an instance of Parser class
using (Parser parser = new Parser(filePath))
{
    // Check if the document supports hyperlink extraction
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Extract hyperlinks from the document
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks();
    // Iterate over hyperlinks
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Print the hyperlink text
        Console.WriteLine(h.Text);
        // Print the hyperlink URL
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### See Also

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int) {#gethyperlinks_2}

Extracts hyperlinks from the document page.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | The zero-based page index. |

### Return Value

A collection of [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objects; `null` if hyperlinks extraction isn't supported.

### Examples

The following example shows how to extract hyperlinks from the document page:

```csharp
// Create an instance of Parser class
using (Parser parser = new Parser(filePath))
{
    // Check if the document supports hyperlink extraction
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Get the document info
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Check if the document has pages
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    // Iterate over pages
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Print a page number 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Extract hyperlinks from the document page
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex);
        // Iterate over hyperlinks
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Print the hyperlink text
            Console.WriteLine(h.Text);
            // Print the hyperlink URL
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
    }
}
```

### See Also

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(PageAreaOptions) {#gethyperlinks_1}

Extracts hyperlinks from the document using customization options (to set the rectangular area that contains hyperlinks).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(PageAreaOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| options | PageAreaOptions | The options for hyperlinks extraction. |

### Return Value

A collection of [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objects; `null` if hyperlinks extraction isn't supported.

### Examples

The following example shows how to extract hyperlinks from the document page area:

```csharp
// Create an instance of Parser class
using (Parser parser = new Parser(filePath))
{
    // Check if the document supports hyperlink extraction
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Create the options which are used for hyperlink extraction
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Extract hyperlinks from the document page area
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(options);
    // Iterate over hyperlinks
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Print the hyperlink text
        Console.WriteLine(h.Text);
        // Print the hyperlink URL
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### See Also

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int, PageAreaOptions) {#gethyperlinks_3}

Extracts hyperlinks from the document page using customization options (to set the rectangular area that contains hyperlinks).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex, PageAreaOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | The zero-based page index. |
| options | PageAreaOptions | The options for hyperlinks extraction. |

### Return Value

A collection of [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objects; `null` if hyperlinks extraction isn't supported.

### Examples

The following example shows how to extract hyperlinks from the document page area using customization options:

```csharp
// Create an instance of Parser class
using (Parser parser = new Parser(filePath))
{
    // Check if the document supports hyperlink extraction
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    
    // Get the document info
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Check if the document has pages
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // Create the options which are used for hyperlink extraction
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Iterate over pages
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Print a page number 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));         
        // Extract hyperlinks from the document page area
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex, options);
        // Iterate over hyperlinks
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Print the hyperlink text
            Console.WriteLine(h.Text);
            // Print the hyperlink URL
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
}
```

### See Also

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.parser.dll -->

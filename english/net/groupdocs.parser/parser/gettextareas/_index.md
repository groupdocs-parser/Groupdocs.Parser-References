---
title: GetTextAreas
second_title: GroupDocs.Parser for .NET API Reference
description: Extracts text areas from the document.
type: docs
weight: 160
url: /net/groupdocs.parser/parser/gettextareas/
---
## GetTextAreas() {#gettextareas}

Extracts text areas from the document.

```csharp
public IEnumerable<PageTextArea> GetTextAreas()
```

### Return Value

A collection of [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objects; `null` if text areas extraction isn't supported.

### Remarks

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Examples

The following example shows how to extract all text areas from the whole document:

```csharp
// Create an instance of Parser class
using(Parser parser = new Parser(filePath))
{
    // Extract text areas
    IEnumerable<PageTextArea> areas = parser.GetTextAreas();
    // Check if text areas extraction is supported
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Iterate over page text areas
    foreach(PageTextArea a in areas)
    {
        // Print a page index, rectangle and text area value:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### See Also

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(PageTextAreaOptions) {#gettextareas_1}

Extracts text areas from the document using customization options (regular expression, match case, etc.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(PageTextAreaOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| options | PageTextAreaOptions | The options for text area extraction. |

### Return Value

A collection of [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objects; `null` if text areas extraction isn't supported.

### Remarks

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Examples

The following example shows how to extract only text areas with digits from the upper-left courner:

```csharp
// Create an instance of Parser class
using(Parser parser = new Parser(filePath))
{
    // Create the options which are used for text area extraction
    PageTextAreaOptions options = new PageTextAreaOptions("[0-9]+", new Rectangle(new Point(0, 0), new Size(300, 100)));

    // Extract text areas which contain only digits from the upper-left courner of a page:
    IEnumerable<PageTextArea> areas = parser.GetTextAreas(options);
    // Check if text areas extraction is supported
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Iterate over page text areas
    foreach(PageTextArea a in areas)
    {
        // Print a page index, rectangle and text area value:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### See Also

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(int) {#gettextareas_2}

Extracts text areas from the document page.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | The zero-based page index. |

### Return Value

A collection of [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objects; `null` if text areas extraction isn't supported.

### Remarks

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Examples

To extract text areas from a document page the following method is used:

```csharp
// Create an instance of Parser class
using(Parser parser = new Parser(filePath))
{
    // Check if the document supports text areas extraction
    if(!parser.Features.TextAreas)
    {
        Console.WriteLine("Document isn't supports text areas extraction.");
        return;
    }

    // Get the document info
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Check if the document has pages
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Iterate over pages
    for(int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Print a page number 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
 
        // Iterate over page text areas
        // We ignore null-checking as we have checked text areas extraction feature support earlier
        foreach(PageTextArea a in parser.GetTextAreas(pageIndex))
        {
            // Print a rectangle and text area value:
            Console.WriteLine(string.Format("R: {0}, Text: {1}", a.Rectangle, a.Text));
        }
    }
}
```

### See Also

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(int, PageTextAreaOptions) {#gettextareas_3}

Extracts text areas from the document page using customization options (regular expression, match case, etc.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex, PageTextAreaOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | The zero-based page index. |
| options | PageTextAreaOptions | The options for text area extraction. |

### Return Value

A collection of [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objects; `null` if text areas extraction isn't supported.

### Remarks

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### See Also

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.parser.dll -->

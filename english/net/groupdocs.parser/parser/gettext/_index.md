---
title: GetText
second_title: GroupDocs.Parser for .NET API Reference
description: Extracts a text from the document.
type: docs
weight: 150
url: /net/groupdocs.parser/parser/gettext/
---
## GetText() {#gettext}

Extracts a text from the document.

```csharp
public TextReader GetText()
```

### Return Value

An instance of TextReader class with the extracted text; `null` if text extraction isn't supported.

### Remarks

**Learn more:**

* [Extract text from documents](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Examples

The following example shows how to extract a text from a document:

```csharp
// Create an instance of Parser class
using(Parser parser = new Parser(filePath))
{
    // Extract a text into the reader
    using(TextReader reader = parser.GetText())
    {
        // Print a text from the document
        // If text extraction isn't supported, a reader is null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### See Also

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(TextOptions) {#gettext_1}

Extracts a text page from the document using text options (to enable raw fast text extraction mode).

```csharp
public TextReader GetText(TextOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| options | TextOptions | The text extraction options. |

### Return Value

An instance of TextReader class with the extracted text; `null` if text extraction isn't supported.

### Remarks

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Examples

The following example shows how to extract a raw text from a document:

```csharp
// Create an instance of Parser class
using(Parser parser = new Parser(filePath))
{
    // Extract a raw text into the reader
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // Print a text from the document
        // If text extraction isn't supported, a reader is null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### See Also

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

Extracts a text from the document page.

```csharp
public TextReader GetText(int pageIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | The zero-based page index. |

### Return Value

An instance of TextReader class with the extracted text; `null` if text page extraction isn't supported.

### Remarks

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Examples

The following example shows how to extract a text from the document page:

```csharp
// Create an instance of Parser class
using(Parser parser = new Parser(filePath))
{
    // Check if the document supports text extraction
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
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
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // Print a page number 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // Extract a text into the reader
        using(TextReader reader = parser.GetText(p))
        {
            // Print a text from the document
            // We ignore null-checking as we have checked text extraction feature support earlier
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### See Also

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(int, TextOptions) {#gettext_3}

Extracts a text from the document page using text options (to enable raw fast text extraction mode).

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | The zero-based page index. |
| options | TextOptions | The text extraction options. |

### Return Value

An instance of TextReader class with the extracted text; `null` if text page extraction isn't supported.

### Remarks

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Examples

The following example shows how to extract a raw text from the document page:

```csharp
// Create an instance of Parser class
using(Parser parser = new Parser(filePath))
{
    // Check if the document supports text extraction
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Get the document info
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // Check if the document has pages
    if(documentInfo == null || documentInfo.RawPageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Iterate over pages
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // Print a page number 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // Extract a text into the reader
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // Print a text from the document
            // We ignore null-checking as we have checked text extraction feature support earlier
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### See Also

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.parser.dll -->

---
title: GetHyperlinks
second_title: GroupDocs.Parser voor .NET API-referentie
description: Haalt hyperlinks uit het document.
type: docs
weight: 100
url: /nl/net/groupdocs.parser/parser/gethyperlinks/
---
## GetHyperlinks() {#gethyperlinks}

Haalt hyperlinks uit het document.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks()
```

### Winstwaarde

Een verzameling van[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objecten; `nul` als extractie van hyperlinks niet wordt ondersteund.

### Voorbeelden

Het volgende voorbeeld laat zien hoe u alle hyperlinks uit het hele document extraheert:

```csharp
// Maak een instantie van de Parser-klasse
using (Parser parser = new Parser(filePath))
{
    // Controleer of het document hyperlinkextractie ondersteunt
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Extraheer hyperlinks uit het document
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks();
    // Itereren over hyperlinks
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Druk de hyperlinktekst af
        Console.WriteLine(h.Text);
        // Druk de hyperlink-URL af
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Zie ook

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int) {#gethyperlinks_2}

Haalt hyperlinks uit de documentpagina.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageIndex | Int32 | De op nul gebaseerde pagina-index. |

### Winstwaarde

Een verzameling van[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objecten; `nul` als extractie van hyperlinks niet wordt ondersteund.

### Voorbeelden

Het volgende voorbeeld laat zien hoe u hyperlinks uit de documentpagina haalt:

```csharp
// Maak een instantie van de Parser-klasse
using (Parser parser = new Parser(filePath))
{
    // Controleer of het document hyperlinkextractie ondersteunt
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Haal de documentinfo op
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Controleer of het document pagina's heeft
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    // Herhaal pagina's
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Druk een paginanummer af 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Extraheer hyperlinks van de documentpagina
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex);
        // Itereren over hyperlinks
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Druk de hyperlinktekst af
            Console.WriteLine(h.Text);
            // Druk de hyperlink-URL af
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
    }
}
```

### Zie ook

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## GetHyperlinks(PageAreaOptions) {#gethyperlinks_1}

Haalt hyperlinks uit het document met behulp van aanpassingsopties (om het rechthoekige gebied in te stellen dat hyperlinks bevat).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(PageAreaOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| options | PageAreaOptions | De opties voor het extraheren van hyperlinks. |

### Winstwaarde

Een verzameling van[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objecten; `nul` als extractie van hyperlinks niet wordt ondersteund.

### Voorbeelden

In het volgende voorbeeld ziet u hoe u hyperlinks kunt extraheren uit het documentpaginagebied:

```csharp
// Maak een instantie van de Parser-klasse
using (Parser parser = new Parser(filePath))
{
    // Controleer of het document hyperlinkextractie ondersteunt
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Maak de opties die worden gebruikt voor het extraheren van hyperlinks
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Extraheer hyperlinks uit het documentpaginagebied
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(options);
    // Itereren over hyperlinks
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Druk de hyperlinktekst af
        Console.WriteLine(h.Text);
        // Druk de hyperlink-URL af
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Zie ook

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int, PageAreaOptions) {#gethyperlinks_3}

Haalt hyperlinks uit de documentpagina met behulp van aanpassingsopties (om het rechthoekige gebied in te stellen dat hyperlinks bevat).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex, PageAreaOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageIndex | Int32 | De op nul gebaseerde pagina-index. |
| options | PageAreaOptions | De opties voor het extraheren van hyperlinks. |

### Winstwaarde

Een verzameling van[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objecten; `nul` als extractie van hyperlinks niet wordt ondersteund.

### Voorbeelden

Het volgende voorbeeld laat zien hoe u hyperlinks kunt extraheren uit het documentpaginagebied met behulp van aanpassingsopties:

```csharp
// Maak een instantie van de Parser-klasse
using (Parser parser = new Parser(filePath))
{
    // Controleer of het document hyperlinkextractie ondersteunt
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    
    // Haal de documentinfo op
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Controleer of het document pagina's heeft
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // Maak de opties die worden gebruikt voor het extraheren van hyperlinks
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Herhaal pagina's
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Druk een paginanummer af 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));         
        // Extraheer hyperlinks uit het documentpaginagebied
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex, options);
        // Itereren over hyperlinks
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Druk de hyperlinktekst af
            Console.WriteLine(h.Text);
            // Druk de hyperlink-URL af
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
}
```

### Zie ook

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

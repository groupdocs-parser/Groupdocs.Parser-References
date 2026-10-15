---
title: "GetHyperlinks"
second_title: "GroupDocs.Parser voor .NET API-referentie"
description: "Extraheert hyperlinks uit het document."
type: docs
weight: 120
url: /nl/net/groupdocs.parser/parser/gethyperlinks/
---

## GetHyperlinks() {#gethyperlinks}

Extraheert hyperlinks uit het document.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks()
```

### Retourwaarde

Een collectie van [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objecten; `null` als hyperlink-extractie niet wordt ondersteund.

### Voorbeelden

Het volgende voorbeeld toont hoe alle hyperlinks uit het volledige document te extraheren:

```csharp
// Maak een instantie van de Parser‑klasse
using (Parser parser = new Parser(filePath))
{
    // Controleer of het document hyperlink-extractie ondersteunt
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Extraheer hyperlinks uit het document
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks();
    // Itereer over hyperlinks
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Print de hyperlinktekst
        Console.WriteLine(h.Text);
        // Print de hyperlink-URL
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Zie ook

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int) {#gethyperlinks_2}

Extraheert hyperlinks van de documentpagina.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageIndex | Int32 | De nulgebaseerde paginapositie. |

### Retourwaarde

Een collectie van [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objecten; `null` als hyperlink-extractie niet wordt ondersteund.

### Voorbeelden

Het volgende voorbeeld toont hoe hyperlinks uit de documentpagina te extraheren:

```csharp
// Maak een instantie van de Parser‑klasse
using (Parser parser = new Parser(filePath))
{
    // Controleer of het document hyperlink-extractie ondersteunt
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Haal de documentinformatie op
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Controleer of het document pagina's heeft
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    // Itereer over pagina's
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Print een paginanummer 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Extraheer hyperlinks uit de documentpagina
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex);
        // Itereer over hyperlinks
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Print de hyperlinktekst
            Console.WriteLine(h.Text);
            // Print de hyperlink-URL
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
    }
}
```

### Zie ook

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(PageAreaOptions) {#gethyperlinks_1}

Extraheert hyperlinks uit het document met behulp van aanpassingsopties (om het rechthoekige gebied dat hyperlinks bevat in te stellen).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(PageAreaOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| options | PageAreaOptions | De opties voor het extraheren van hyperlinks. |

### Retourwaarde

Een collectie van [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objecten; `null` als hyperlink-extractie niet wordt ondersteund.

### Voorbeelden

Het volgende voorbeeld toont hoe hyperlinks uit het paginagedeelte van het document te extraheren:

```csharp
// Maak een instantie van de Parser‑klasse
using (Parser parser = new Parser(filePath))
{
    // Controleer of het document hyperlink-extractie ondersteunt
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Maak de opties die worden gebruikt voor hyperlink-extractie
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Extraheer hyperlinks uit het paginagedeelte van het document
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(options);
    // Itereer over hyperlinks
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Print de hyperlinktekst
        Console.WriteLine(h.Text);
        // Print de hyperlink-URL
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Zie ook

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int, PageAreaOptions) {#gethyperlinks_3}

Extraheert hyperlinks van de documentpagina met behulp van aanpassingsopties (om het rechthoekige gebied dat hyperlinks bevat in te stellen).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex, PageAreaOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageIndex | Int32 | De nulgebaseerde paginapositie. |
| options | PageAreaOptions | De opties voor het extraheren van hyperlinks. |

### Retourwaarde

Een collectie van [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objecten; `null` als hyperlink-extractie niet wordt ondersteund.

### Voorbeelden

Het volgende voorbeeld laat zien hoe u hyperlinks uit het paginagedeelte van het document kunt extraheren met behulp van aanpassingsopties:

```csharp
// Maak een instantie van de Parser‑klasse
using (Parser parser = new Parser(filePath))
{
    // Controleer of het document hyperlink-extractie ondersteunt
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    
    // Haal de documentinformatie op
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Controleer of het document pagina's heeft
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // Maak de opties die worden gebruikt voor hyperlink-extractie
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Itereer over pagina's
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Print een paginanummer 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));         
        // Extraheer hyperlinks uit het paginagedeelte van het document
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex, options);
        // Itereer over hyperlinks
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Print de hyperlinktekst
            Console.WriteLine(h.Text);
            // Print de hyperlink-URL
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
}
```

### Zie ook

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

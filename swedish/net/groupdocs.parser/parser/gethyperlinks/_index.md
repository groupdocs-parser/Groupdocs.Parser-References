---
title: GetHyperlinks
second_title: GroupDocs.Parser för .NET API-referens
description: Extraherar hyperlänkar från dokumentet.
type: docs
weight: 100
url: /sv/net/groupdocs.parser/parser/gethyperlinks/
---
## GetHyperlinks() {#gethyperlinks}

Extraherar hyperlänkar från dokumentet.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks()
```

### Returvärde

En samling av[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objekt; `null` om extrahering av hyperlänkar inte stöds.

### Exempel

Följande exempel visar hur man extraherar alla hyperlänkar från hela dokumentet:

```csharp
// Skapa en instans av Parser-klassen
using (Parser parser = new Parser(filePath))
{
    // Kontrollera om dokumentet stöder extraktion av hyperlänkar
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Extrahera hyperlänkar från dokumentet
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks();
    // Iterera över hyperlänkar
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Skriv ut hyperlänkstexten
        Console.WriteLine(h.Text);
        // Skriv ut hyperlänkens URL
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Se även

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int) {#gethyperlinks_2}

Extraherar hyperlänkar från dokumentsidan.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | Det nollbaserade sidindexet. |

### Returvärde

En samling av[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objekt; `null` om extrahering av hyperlänkar inte stöds.

### Exempel

Följande exempel visar hur man extraherar hyperlänkar från dokumentsidan:

```csharp
// Skapa en instans av Parser-klassen
using (Parser parser = new Parser(filePath))
{
    // Kontrollera om dokumentet stöder extraktion av hyperlänkar
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Få dokumentinformationen
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Kontrollera om dokumentet har sidor
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    // Iterera över sidor
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Skriv ut ett sidnummer 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Extrahera hyperlänkar från dokumentsidan
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex);
        // Iterera över hyperlänkar
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Skriv ut hyperlänkstexten
            Console.WriteLine(h.Text);
            // Skriv ut hyperlänkens URL
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
    }
}
```

### Se även

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## GetHyperlinks(PageAreaOptions) {#gethyperlinks_1}

Extraherar hyperlänkar från dokumentet med hjälp av anpassningsalternativ (för att ställa in det rektangulära område som innehåller hyperlänkar).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(PageAreaOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| options | PageAreaOptions | Alternativen för extrahering av hyperlänkar. |

### Returvärde

En samling av[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objekt; `null` om extrahering av hyperlänkar inte stöds.

### Exempel

Följande exempel visar hur man extraherar hyperlänkar från dokumentsidans område:

```csharp
// Skapa en instans av Parser-klassen
using (Parser parser = new Parser(filePath))
{
    // Kontrollera om dokumentet stöder extraktion av hyperlänkar
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Skapa alternativen som används för extrahering av hyperlänkar
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Extrahera hyperlänkar från dokumentsidans område
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(options);
    // Iterera över hyperlänkar
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Skriv ut hyperlänkstexten
        Console.WriteLine(h.Text);
        // Skriv ut hyperlänkens URL
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Se även

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int, PageAreaOptions) {#gethyperlinks_3}

Extraherar hyperlänkar från dokumentsidan med hjälp av anpassningsalternativ (för att ställa in det rektangulära område som innehåller hyperlänkar).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex, PageAreaOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | Det nollbaserade sidindexet. |
| options | PageAreaOptions | Alternativen för extrahering av hyperlänkar. |

### Returvärde

En samling av[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objekt; `null` om extrahering av hyperlänkar inte stöds.

### Exempel

Följande exempel visar hur man extraherar hyperlänkar från dokumentsidans område med hjälp av anpassningsalternativ:

```csharp
// Skapa en instans av Parser-klassen
using (Parser parser = new Parser(filePath))
{
    // Kontrollera om dokumentet stöder extraktion av hyperlänkar
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    
    // Få dokumentinformationen
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Kontrollera om dokumentet har sidor
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // Skapa alternativen som används för extrahering av hyperlänkar
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Iterera över sidor
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Skriv ut ett sidnummer 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));         
        // Extrahera hyperlänkar från dokumentsidans område
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex, options);
        // Iterera över hyperlänkar
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Skriv ut hyperlänkstexten
            Console.WriteLine(h.Text);
            // Skriv ut hyperlänkens URL
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
}
```

### Se även

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

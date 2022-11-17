---
title: GetImages
second_title: GroupDocs.Parser för .NET API-referens
description: Extraherar bilder från dokumentet.
type: docs
weight: 110
url: /sv/net/groupdocs.parser/parser/getimages/
---
## GetImages() {#getimages}

Extraherar bilder från dokumentet.

```csharp
public IEnumerable<PageImageArea> GetImages()
```

### Returvärde

En samling av[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) objekt; `null` om bildextraktion inte stöds.

### Anmärkningar

**Läs mer:**

* [Extrahera bilder från dokument](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extrahera bilder till filer](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extrahera bilder från Microsoft Office Word-dokument](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extrahera bilder från Microsoft Office Excel-kalkylblad](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extrahera bilder från Microsoft Office PowerPoint-presentationer](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extrahera bilder från e-postmeddelanden](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extrahera bilder från PDF-dokument](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Exempel

Följande exempel visar hur man extraherar alla bilder från hela dokumentet:

```csharp
// Skapa en instans av Parser-klassen
using (Parser parser = new Parser(filePath))
{
    // Extrahera bilder
    IEnumerable<PageImageArea> images = parser.GetImages();
    // Kontrollera om bildextraktion stöds
    if (images == null)
    {
        Console.WriteLine("Images extraction isn't supported");
        return;
    }
    // Iterera över bilder
    foreach (PageImageArea image in images)
    {
        // Skriv ut ett sidindex, rektangel och bildtyp:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Se även

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## GetImages(PageAreaOptions) {#getimages_1}

Extraherar bilder från dokumentet med hjälp av anpassningsalternativ (för att ställa in det rektangulära område som innehåller bilder).

```csharp
public IEnumerable<PageImageArea> GetImages(PageAreaOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| options | PageAreaOptions | Alternativen för att extrahera bilder. |

### Returvärde

En samling av[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) objekt; `null` om bildextraktion inte stöds.

### Anmärkningar

**Läs mer:**

* [Extrahera bilder från dokument](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extrahera bilder till filer](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extrahera bilder från dokumentsidans område](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extrahera bilder från Microsoft Office Word-dokument](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extrahera bilder från Microsoft Office Excel-kalkylblad](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extrahera bilder från Microsoft Office PowerPoint-presentationer](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extrahera bilder från e-postmeddelanden](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extrahera bilder från PDF-dokument](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Exempel

Följande exempel visar hur man extraherar endast bilder från det övre vänstra fältet:

```csharp
// Skapa en instans av Parser-klassen
using (Parser parser = new Parser(filePath))
{
    // Skapa alternativen som används för att extrahera bilder
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(0, 0), new Size(300, 100)));
    // Extrahera bilder från det övre vänstra hörnet på en sida:
    IEnumerable<PageImageArea> images = parser.GetImages(options);
    // Kontrollera om bildextraktion stöds
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }
    // Iterera över bilder
    foreach (PageImageArea image in images)
    {
        // Skriv ut ett sidindex, rektangel och bildtyp:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Se även

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## GetImages(int) {#getimages_2}

Extraherar bilder från dokumentsidan.

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | Det nollbaserade sidindexet. |

### Returvärde

En samling av[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) objekt; `null` om bildextraktion inte stöds.

### Anmärkningar

**Läs mer:**

* [Extrahera bilder från dokument](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extrahera bilder till filer](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extrahera bilder från dokumentsidan](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extrahera bilder från Microsoft Office Word-dokument](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extrahera bilder från Microsoft Office Excel-kalkylblad](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extrahera bilder från Microsoft Office PowerPoint-presentationer](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extrahera bilder från e-postmeddelanden](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extrahera bilder från PDF-dokument](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Exempel

För att extrahera bilder från en dokumentsida används följande metod:

```csharp
// Skapa en instans av Parser-klassen
using (Parser parser = new Parser(filePath))
{
    // Kontrollera om dokumentet stöder extrahering av bilder
    if (!parser.Features.Images)
    {
        Console.WriteLine("Document isn't supports images extraction.");
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
    for (int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Skriv ut ett sidnummer 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Iterera över bilder
        // Vi ignorerar nollkontroll eftersom vi har kontrollerat stöd för bildextraktion tidigare
        foreach (PageImageArea image in parser.GetImages(pageIndex))
        {
            // Skriv ut en rektangel och bildtyp
            Console.WriteLine(string.Format("R: {0}, Text: {1}", image.Rectangle, image.FileType));
        }
    }
}
```

### Se även

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## GetImages(int, PageAreaOptions) {#getimages_3}

Extraherar bilder från dokumentsidan med hjälp av anpassningsalternativ (för att ställa in det rektangulära område som innehåller bilder).

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex, PageAreaOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | Det nollbaserade sidindexet. |
| options | PageAreaOptions | Alternativen för att extrahera bilder. |

### Returvärde

En samling av[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) objekt; `null` om bildextraktion inte stöds.

### Anmärkningar

**Läs mer:**

* [Extrahera bilder från dokument](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extrahera bilder till filer](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extrahera bilder från dokumentsidan](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extrahera bilder från dokumentsidans område](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extrahera bilder från Microsoft Office Word-dokument](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extrahera bilder från Microsoft Office Excel-kalkylblad](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extrahera bilder från Microsoft Office PowerPoint-presentationer](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extrahera bilder från e-postmeddelanden](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extrahera bilder från PDF-dokument](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Se även

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

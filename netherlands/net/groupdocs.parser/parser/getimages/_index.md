---
title: GetImages
second_title: GroupDocs.Parser voor .NET API-referentie
description: Haalt afbeeldingen uit het document.
type: docs
weight: 110
url: /nl/net/groupdocs.parser/parser/getimages/
---
## GetImages() {#getimages}

Haalt afbeeldingen uit het document.

```csharp
public IEnumerable<PageImageArea> GetImages()
```

### Winstwaarde

Een verzameling van[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) objecten; `nul` als het extraheren van afbeeldingen niet wordt ondersteund.

### Opmerkingen

**Kom meer te weten:**

* [Extraheer afbeeldingen uit documenten](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extraheer afbeeldingen naar bestanden](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extraheer afbeeldingen uit Microsoft Office Word-documenten](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extraheer afbeeldingen uit Microsoft Office Excel-spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extraheer afbeeldingen uit Microsoft Office PowerPoint-presentaties](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extraheer afbeeldingen uit e-mails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extraheer afbeeldingen uit PDF-documenten](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Voorbeelden

Het volgende voorbeeld laat zien hoe u alle afbeeldingen uit het hele document kunt extraheren:

```csharp
// Maak een instantie van de Parser-klasse
using (Parser parser = new Parser(filePath))
{
    // Extraheer afbeeldingen
    IEnumerable<PageImageArea> images = parser.GetImages();
    // Controleer of het extraheren van afbeeldingen wordt ondersteund
    if (images == null)
    {
        Console.WriteLine("Images extraction isn't supported");
        return;
    }
    // Itereren over afbeeldingen
    foreach (PageImageArea image in images)
    {
        // Druk een pagina-index, rechthoek en afbeeldingstype af:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Zie ook

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## GetImages(PageAreaOptions) {#getimages_1}

Haalt afbeeldingen uit het document met behulp van aanpassingsopties (om het rechthoekige gebied in te stellen dat afbeeldingen bevat).

```csharp
public IEnumerable<PageImageArea> GetImages(PageAreaOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| options | PageAreaOptions | De opties voor het extraheren van afbeeldingen. |

### Winstwaarde

Een verzameling van[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) objecten; `nul` als het extraheren van afbeeldingen niet wordt ondersteund.

### Opmerkingen

**Kom meer te weten:**

* [Extraheer afbeeldingen uit documenten](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extraheer afbeeldingen naar bestanden](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extraheer afbeeldingen uit het documentpaginagebied](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extraheer afbeeldingen uit Microsoft Office Word-documenten](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extraheer afbeeldingen uit Microsoft Office Excel-spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extraheer afbeeldingen uit Microsoft Office PowerPoint-presentaties](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extraheer afbeeldingen uit e-mails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extraheer afbeeldingen uit PDF-documenten](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Voorbeelden

Het volgende voorbeeld laat zien hoe u alleen afbeeldingen uit de linkerbovenhoek haalt:

```csharp
// Maak een instantie van de Parser-klasse
using (Parser parser = new Parser(filePath))
{
    // Maak de opties die worden gebruikt voor het extraheren van afbeeldingen
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(0, 0), new Size(300, 100)));
    // Extraheer afbeeldingen uit de linkerbovenhoek van een pagina:
    IEnumerable<PageImageArea> images = parser.GetImages(options);
    // Controleer of het extraheren van afbeeldingen wordt ondersteund
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }
    // Itereren over afbeeldingen
    foreach (PageImageArea image in images)
    {
        // Druk een pagina-index, rechthoek en afbeeldingstype af:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Zie ook

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## GetImages(int) {#getimages_2}

Haalt afbeeldingen uit de documentpagina.

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageIndex | Int32 | De op nul gebaseerde pagina-index. |

### Winstwaarde

Een verzameling van[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) objecten; `nul` als het extraheren van afbeeldingen niet wordt ondersteund.

### Opmerkingen

**Kom meer te weten:**

* [Extraheer afbeeldingen uit documenten](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extraheer afbeeldingen naar bestanden](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Haal afbeeldingen uit de documentpagina](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extraheer afbeeldingen uit Microsoft Office Word-documenten](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extraheer afbeeldingen uit Microsoft Office Excel-spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extraheer afbeeldingen uit Microsoft Office PowerPoint-presentaties](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extraheer afbeeldingen uit e-mails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extraheer afbeeldingen uit PDF-documenten](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Voorbeelden

Om afbeeldingen uit een documentpagina te extraheren, wordt de volgende methode gebruikt:

```csharp
// Maak een instantie van de Parser-klasse
using (Parser parser = new Parser(filePath))
{
    // Controleer of het document het extraheren van afbeeldingen ondersteunt
    if (!parser.Features.Images)
    {
        Console.WriteLine("Document isn't supports images extraction.");
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
    for (int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Druk een paginanummer af 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Itereren over afbeeldingen
        // We negeren null-check omdat we de ondersteuning voor het extraheren van afbeeldingen eerder hebben gecontroleerd
        foreach (PageImageArea image in parser.GetImages(pageIndex))
        {
            // Druk een rechthoek en afbeeldingstype af
            Console.WriteLine(string.Format("R: {0}, Text: {1}", image.Rectangle, image.FileType));
        }
    }
}
```

### Zie ook

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## GetImages(int, PageAreaOptions) {#getimages_3}

Haalt afbeeldingen uit de documentpagina met behulp van aanpassingsopties (om het rechthoekige gebied in te stellen dat afbeeldingen bevat).

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex, PageAreaOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageIndex | Int32 | De op nul gebaseerde pagina-index. |
| options | PageAreaOptions | De opties voor het extraheren van afbeeldingen. |

### Winstwaarde

Een verzameling van[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) objecten; `nul` als het extraheren van afbeeldingen niet wordt ondersteund.

### Opmerkingen

**Kom meer te weten:**

* [Extraheer afbeeldingen uit documenten](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extraheer afbeeldingen naar bestanden](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Haal afbeeldingen uit de documentpagina](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extraheer afbeeldingen uit het documentpaginagebied](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extraheer afbeeldingen uit Microsoft Office Word-documenten](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extraheer afbeeldingen uit Microsoft Office Excel-spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extraheer afbeeldingen uit Microsoft Office PowerPoint-presentaties](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extraheer afbeeldingen uit e-mails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extraheer afbeeldingen uit PDF-documenten](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Zie ook

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

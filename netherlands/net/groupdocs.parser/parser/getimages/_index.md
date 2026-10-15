---
title: "GetImages"
second_title: "GroupDocs.Parser voor .NET API-referentie"
description: "Extraheert afbeeldingen uit het document."
type: docs
weight: 130
url: /nl/net/groupdocs.parser/parser/getimages/
---

## GetImages() {#getimages}

Extraheert afbeeldingen uit het document.

```csharp
public IEnumerable<PageImageArea> GetImages()
```

### Retourwaarde

Een verzameling van [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea)-objecten; `null` als het extraheren van afbeeldingen niet wordt ondersteund.

### Opmerkingen

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Voorbeelden

Het volgende voorbeeld toont hoe je alle afbeeldingen uit het volledige document kunt extraheren:

```csharp
// Maak een instantie van de Parser‑klasse
using (Parser parser = new Parser(filePath))
{
    // Afbeeldingen extraheren
    IEnumerable<PageImageArea> images = parser.GetImages();
    // Controleren of het extraheren van afbeeldingen wordt ondersteund
    if (images == null)
    {
        Console.WriteLine("Images extraction isn't supported");
        return;
    }
    // Itereren over afbeeldingen
    foreach (PageImageArea image in images)
    {
        // Print een paginapositie, rechthoek en afbeeldingstype:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Zie ook

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(PageAreaOptions) {#getimages_1}

Extraheert afbeeldingen uit het document met behulp van aanpassingsopties (om het rechthoekige gebied dat afbeeldingen bevat in te stellen).

```csharp
public IEnumerable<PageImageArea> GetImages(PageAreaOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| options | PageAreaOptions | De opties voor het extraheren van afbeeldingen. |

### Retourwaarde

Een verzameling van [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea)-objecten; `null` als het extraheren van afbeeldingen niet wordt ondersteund.

### Opmerkingen

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page area](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Voorbeelden

Het volgende voorbeeld toont hoe je alleen afbeeldingen uit de linkerbovenhoek kunt extraheren:

```csharp
// Maak een instantie van de Parser‑klasse
using (Parser parser = new Parser(filePath))
{
    // Maak de opties aan die worden gebruikt voor het extraheren van afbeeldingen
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(0, 0), new Size(300, 100)));
    // Afbeeldingen extraheren uit de linkerbovenhoek van een pagina:
    IEnumerable<PageImageArea> images = parser.GetImages(options);
    // Controleren of het extraheren van afbeeldingen wordt ondersteund
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }
    // Itereren over afbeeldingen
    foreach (PageImageArea image in images)
    {
        // Print een paginapositie, rechthoek en afbeeldingstype:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Zie ook

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(int) {#getimages_2}

Extraheert afbeeldingen van de documentpagina.

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageIndex | Int32 | De nulgebaseerde paginapositie. |

### Retourwaarde

Een verzameling van [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea)-objecten; `null` als het extraheren van afbeeldingen niet wordt ondersteund.

### Opmerkingen

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Voorbeelden

Om afbeeldingen uit een documentpagina te extraheren wordt de volgende methode gebruikt:

```csharp
// Maak een instantie van de Parser‑klasse
using (Parser parser = new Parser(filePath))
{
    // Controleer of het document het extraheren van afbeeldingen ondersteunt
    if (!parser.Features.Images)
    {
        Console.WriteLine("Document isn't supports images extraction.");
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
    for (int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Print een paginanummer 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Itereren over afbeeldingen
        // We negeren null-controle omdat we eerder de ondersteuning van de afbeeldingsextractiefunctie hebben gecontroleerd
        foreach (PageImageArea image in parser.GetImages(pageIndex))
        {
            // Print een rechthoek en afbeeldingstype
            Console.WriteLine(string.Format("R: {0}, Text: {1}", image.Rectangle, image.FileType));
        }
    }
}
```

### Zie ook

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(int, PageAreaOptions) {#getimages_3}

Extraheert afbeeldingen van de documentpagina met behulp van aanpassingsopties (om het rechthoekige gebied dat afbeeldingen bevat in te stellen).

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex, PageAreaOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageIndex | Int32 | De nulgebaseerde paginapositie. |
| options | PageAreaOptions | De opties voor het extraheren van afbeeldingen. |

### Retourwaarde

Een verzameling van [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea)-objecten; `null` als het extraheren van afbeeldingen niet wordt ondersteund.

### Opmerkingen

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extract images from document page area](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Zie ook

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

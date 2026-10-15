---
title: "GetImages"
second_title: "Riferimento API di GroupDocs.Parser per .NET"
description: "Estrae le immagini dal documento."
type: docs
weight: 130
url: /it/net/groupdocs.parser/parser/getimages/
---

## GetImages() {#getimages}

Estrae le immagini dal documento.

```csharp
public IEnumerable<PageImageArea> GetImages()
```

### Valore di ritorno

Una collezione di oggetti [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea); `null` se l'estrazione delle immagini non è supportata.

### Osservazioni

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Esempi

Il seguente esempio mostra come estrarre tutte le immagini dall'intero documento:

```csharp
// Crea un'istanza della classe Parser
using (Parser parser = new Parser(filePath))
{
    // Estrai immagini
    IEnumerable<PageImageArea> images = parser.GetImages();
    // Verifica se l'estrazione delle immagini è supportata
    if (images == null)
    {
        Console.WriteLine("Images extraction isn't supported");
        return;
    }
    // Itera sulle immagini
    foreach (PageImageArea image in images)
    {
        // Stampa l'indice della pagina, il rettangolo e il tipo di immagine:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Vedi anche

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(PageAreaOptions) {#getimages_1}

Estrae le immagini dal documento utilizzando le opzioni di personalizzazione (per impostare l'area rettangolare che contiene le immagini).

```csharp
public IEnumerable<PageImageArea> GetImages(PageAreaOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| options | PageAreaOptions | Le opzioni per l'estrazione delle immagini. |

### Valore di ritorno

Una collezione di oggetti [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea); `null` se l'estrazione delle immagini non è supportata.

### Osservazioni

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page area](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Esempi

Il seguente esempio mostra come estrarre solo le immagini dall'angolo in alto a sinistra:

```csharp
// Crea un'istanza della classe Parser
using (Parser parser = new Parser(filePath))
{
    // Crea le opzioni utilizzate per l'estrazione delle immagini
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(0, 0), new Size(300, 100)));
    // Estrai le immagini dall'angolo in alto a sinistra di una pagina:
    IEnumerable<PageImageArea> images = parser.GetImages(options);
    // Verifica se l'estrazione delle immagini è supportata
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }
    // Itera sulle immagini
    foreach (PageImageArea image in images)
    {
        // Stampa l'indice della pagina, il rettangolo e il tipo di immagine:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Vedi anche

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(int) {#getimages_2}

Estrae le immagini dalla pagina del documento.

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | L'indice di pagina basato su zero. |

### Valore di ritorno

Una collezione di oggetti [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea); `null` se l'estrazione delle immagini non è supportata.

### Osservazioni

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Esempi

Per estrarre le immagini da una pagina di documento viene utilizzato il seguente metodo:

```csharp
// Crea un'istanza della classe Parser
using (Parser parser = new Parser(filePath))
{
    // Verifica se il documento supporta l'estrazione delle immagini
    if (!parser.Features.Images)
    {
        Console.WriteLine("Document isn't supports images extraction.");
        return;
    }
    
    // Ottieni le informazioni del documento
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Verifica se il documento ha pagine
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // Itera sulle pagine
    for (int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Stampa un numero di pagina 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Itera sulle immagini
        // Ignoriamo il controllo di null poiché abbiamo già verificato il supporto della funzionalità di estrazione delle immagini
        foreach (PageImageArea image in parser.GetImages(pageIndex))
        {
            // Stampa un rettangolo e il tipo di immagine
            Console.WriteLine(string.Format("R: {0}, Text: {1}", image.Rectangle, image.FileType));
        }
    }
}
```

### Vedi anche

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(int, PageAreaOptions) {#getimages_3}

Estrae le immagini dalla pagina del documento utilizzando le opzioni di personalizzazione (per impostare l'area rettangolare che contiene le immagini).

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex, PageAreaOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | L'indice di pagina basato su zero. |
| options | PageAreaOptions | Le opzioni per l'estrazione delle immagini. |

### Valore di ritorno

Una collezione di oggetti [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea); `null` se l'estrazione delle immagini non è supportata.

### Osservazioni

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

### Vedi anche

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

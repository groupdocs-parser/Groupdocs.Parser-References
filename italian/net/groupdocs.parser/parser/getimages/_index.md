---
title: GetImages
second_title: Riferimento API GroupDocs.Parser per .NET
description: Estrae le immagini dal documento.
type: docs
weight: 110
url: /it/net/groupdocs.parser/parser/getimages/
---
## GetImages() {#getimages}

Estrae le immagini dal documento.

```csharp
public IEnumerable<PageImageArea> GetImages()
```

### Valore di ritorno

Una raccolta di[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) oggetti; `nullo` se l'estrazione delle immagini non è supportata.

### Osservazioni

**Saperne di più:**

* [Estrai immagini dai documenti](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Estrai immagini in file](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Estrai immagini da documenti Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Estrai immagini da fogli di calcolo di Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Estrai immagini da presentazioni di Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Estrai le immagini dalle e-mail](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Estrai immagini da documenti PDF](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Esempi

L'esempio seguente mostra come estrarre tutte le immagini dall'intero documento:

```csharp
// Crea un'istanza della classe Parser
using (Parser parser = new Parser(filePath))
{
    // Estrai le immagini
    IEnumerable<PageImageArea> images = parser.GetImages();
    // Controlla se l'estrazione delle immagini è supportata
    if (images == null)
    {
        Console.WriteLine("Images extraction isn't supported");
        return;
    }
    // Itera sulle immagini
    foreach (PageImageArea image in images)
    {
        // Stampa un indice di pagina, un rettangolo e un tipo di immagine:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Guarda anche

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

---

## GetImages(PageAreaOptions) {#getimages_1}

Estrae le immagini dal documento utilizzando le opzioni di personalizzazione (per impostare l'area rettangolare che contiene le immagini).

```csharp
public IEnumerable<PageImageArea> GetImages(PageAreaOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| options | PageAreaOptions | Le opzioni per l'estrazione delle immagini. |

### Valore di ritorno

Una raccolta di[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) oggetti; `nullo` se l'estrazione delle immagini non è supportata.

### Osservazioni

**Saperne di più:**

* [Estrai immagini dai documenti](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Estrai immagini in file](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Estrai le immagini dall'area della pagina del documento](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Estrai immagini da documenti Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Estrai immagini da fogli di calcolo di Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Estrai immagini da presentazioni di Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Estrai le immagini dalle e-mail](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Estrai immagini da documenti PDF](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Esempi

L'esempio seguente mostra come estrarre solo le immagini dall'angolo in alto a sinistra:

```csharp
// Crea un'istanza della classe Parser
using (Parser parser = new Parser(filePath))
{
    // Crea le opzioni utilizzate per l'estrazione delle immagini
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(0, 0), new Size(300, 100)));
    // Estrai le immagini dall'angolo in alto a sinistra di una pagina:
    IEnumerable<PageImageArea> images = parser.GetImages(options);
    // Controlla se l'estrazione delle immagini è supportata
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }
    // Itera sulle immagini
    foreach (PageImageArea image in images)
    {
        // Stampa un indice di pagina, un rettangolo e un tipo di immagine:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Guarda anche

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

---

## GetImages(int) {#getimages_2}

Estrae le immagini dalla pagina del documento.

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | L'indice della pagina in base zero. |

### Valore di ritorno

Una raccolta di[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) oggetti; `nullo` se l'estrazione delle immagini non è supportata.

### Osservazioni

**Saperne di più:**

* [Estrai immagini dai documenti](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Estrai immagini in file](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Estrai le immagini dalla pagina del documento](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Estrai immagini da documenti Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Estrai immagini da fogli di calcolo di Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Estrai immagini da presentazioni di Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Estrai le immagini dalle e-mail](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Estrai immagini da documenti PDF](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Esempi

Per estrarre immagini da una pagina di un documento viene utilizzato il seguente metodo:

```csharp
// Crea un'istanza della classe Parser
using (Parser parser = new Parser(filePath))
{
    // Controlla se il documento supporta l'estrazione delle immagini
    if (!parser.Features.Images)
    {
        Console.WriteLine("Document isn't supports images extraction.");
        return;
    }
    
    // Ottieni le informazioni sul documento
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Controlla se il documento ha pagine
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
        // Ignoriamo il controllo null poiché abbiamo verificato in precedenza il supporto della funzione di estrazione delle immagini
        foreach (PageImageArea image in parser.GetImages(pageIndex))
        {
            // Stampa un rettangolo e un tipo di immagine
            Console.WriteLine(string.Format("R: {0}, Text: {1}", image.Rectangle, image.FileType));
        }
    }
}
```

### Guarda anche

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

---

## GetImages(int, PageAreaOptions) {#getimages_3}

Estrae le immagini dalla pagina del documento utilizzando le opzioni di personalizzazione (per impostare l'area rettangolare che contiene le immagini).

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex, PageAreaOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | L'indice della pagina in base zero. |
| options | PageAreaOptions | Le opzioni per l'estrazione delle immagini. |

### Valore di ritorno

Una raccolta di[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) oggetti; `nullo` se l'estrazione delle immagini non è supportata.

### Osservazioni

**Saperne di più:**

* [Estrai immagini dai documenti](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Estrai immagini in file](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Estrai le immagini dalla pagina del documento](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Estrai le immagini dall'area della pagina del documento](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Estrai immagini da documenti Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Estrai immagini da fogli di calcolo di Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Estrai immagini da presentazioni di Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Estrai le immagini dalle e-mail](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Estrai immagini da documenti PDF](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Guarda anche

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

---
title: GetImageStream
second_title: Riferimento API GroupDocs.Parser per .NET
description: Restituisce il flusso di immagini.
type: docs
weight: 40
url: /it/net/groupdocs.parser.data/pageimagearea/getimagestream/
---
## GetImageStream() {#getimagestream}

Restituisce il flusso di immagini.

```csharp
public Stream GetImageStream()
```

### Valore di ritorno

Un flusso con l'immagine.

### Esempi

L'esempio seguente mostra come salvare le immagini su file:

```csharp
// Crea un'istanza della classe Parser
using (Parser parser = new Parser(filePath))
{
    // Estrai le immagini dal documento
    IEnumerable<PageImageArea> images = parser.GetImages();
    
    // Controlla se l'estrazione delle immagini è supportata
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }

    // Itera sulle immagini
    foreach (PageImageArea image in images)
    {
        // Apre il flusso di immagini
        using (Stream imageStream = image.GetImageStream())
        {
            // Crea il file per salvare l'immagine
            using (Stream destStream = File.Create(Guid.NewGuid().ToString() + image.FileType.Extension))
            {
                byte[] buffer = new byte[4096];
                int readed = 0;

                do
                {
                    // Legge i dati dal flusso di immagini
                    readed = imageStream.Read(buffer, 0, buffer.Length);

                    if (readed > 0)
                    {
                        // Scrive i dati nel flusso di file
                        destStream.Write(buffer, 0, readed);
                    }
                }
                while (readed > 0);
            }
        }
    }
}
```

### Guarda anche

* class [PageImageArea](../../pageimagearea)
* spazio dei nomi [GroupDocs.Parser.Data](../../pageimagearea)
* assemblea [GroupDocs.Parser](../../../)

---

## GetImageStream(ImageOptions) {#getimagestream_1}

Restituisce il flusso di immagini in un formato diverso.

```csharp
public Stream GetImageStream(ImageOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| options | ImageOptions | Le opzioni utilizzate per estrarre l'immagine. |

### Valore di ritorno

Un flusso con l'immagine.

### Esempi

L'esempio seguente mostra come salvare le immagini su file in un formato diverso:

```csharp
// Crea un'istanza della classe Parser
using (Parser parser = new Parser(filePath))
{
    // Estrai le immagini dal documento
    IEnumerable<PageImageArea> images = parser.GetImages();
    
    // Controlla se l'estrazione delle immagini è supportata
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }

    // Crea le opzioni per salvare le immagini in formato PNG
    ImageOptions options = new ImageOptions(ImageFormat.Png);
    
    // Itera sulle immagini
    foreach (PageImageArea image in images)
    {
        // Apre il flusso di immagini
        using (Stream imageStream = image.GetImageStream(options))
        {
            // Crea il file per salvare l'immagine
            using (Stream destStream = File.Create(Guid.NewGuid().ToString() + ".png"))
            {
                byte[] buffer = new byte[4096];
                int readed = 0;

                do
                {
                    // Legge i dati dal flusso di immagini
                    readed = imageStream.Read(buffer, 0, buffer.Length);

                    if (readed > 0)
                    {
                        // Scrive i dati nel flusso di file
                        destStream.Write(buffer, 0, readed);
                    }
                }
                while (readed > 0);
            }
        }
    }
}
```

### Guarda anche

* class [ImageOptions](../../../groupdocs.parser.options/imageoptions)
* class [PageImageArea](../../pageimagearea)
* spazio dei nomi [GroupDocs.Parser.Data](../../pageimagearea)
* assemblea [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
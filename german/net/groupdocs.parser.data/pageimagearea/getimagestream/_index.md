---
title: "GetImageStream"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Gibt den Bild-Stream zurück."
type: docs
weight: 40
url: /de/net/groupdocs.parser.data/pageimagearea/getimagestream/
---

## GetImageStream() {#getimagestream}

Gibt den Bild-Stream zurück.

```csharp
public Stream GetImageStream()
```

### Rückgabewert

Ein Stream mit dem Bild.

### Beispiele

Das folgende Beispiel zeigt, wie Bilder in Dateien gespeichert werden:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using (Parser parser = new Parser(filePath))
{
    // Bilder aus dem Dokument extrahieren
    IEnumerable<PageImageArea> images = parser.GetImages();
    
    // Prüfen, ob die Bildextraktion unterstützt wird
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }

    // Über Bilder iterieren
    foreach (PageImageArea image in images)
    {
        // Den Bild-Stream öffnen
        using (Stream imageStream = image.GetImageStream())
        {
            // Die Datei zum Speichern des Bildes erstellen
            using (Stream destStream = File.Create(Guid.NewGuid().ToString() + image.FileType.Extension))
            {
                byte[] buffer = new byte[4096];
                int readed = 0;

                do
                {
                    // Daten aus dem Bild-Stream lesen
                    readed = imageStream.Read(buffer, 0, buffer.Length);

                    if (readed > 0)
                    {
                        // Daten in den Datei-Stream schreiben
                        destStream.Write(buffer, 0, readed);
                    }
                }
                while (readed > 0);
            }
        }
    }
}
```

### Siehe auch

* class [PageImageArea](../../pageimagearea)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

---

## GetImageStream(ImageOptions) {#getimagestream_1}

Gibt den Bild-Stream in einem anderen Format zurück.

```csharp
public Stream GetImageStream(ImageOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | ImageOptions | Die Optionen, die zum Extrahieren des Bildes verwendet werden. |

### Rückgabewert

Ein Stream mit dem Bild.

### Beispiele

Das folgende Beispiel zeigt, wie Bilder in Dateien in einem anderen Format gespeichert werden:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using (Parser parser = new Parser(filePath))
{
    // Bilder aus dem Dokument extrahieren
    IEnumerable<PageImageArea> images = parser.GetImages();
    
    // Prüfen, ob die Bildextraktion unterstützt wird
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }

    // Erstelle die Optionen, um Bilder im PNG-Format zu speichern
    ImageOptions options = new ImageOptions(ImageFormat.Png);
    
    // Über Bilder iterieren
    foreach (PageImageArea image in images)
    {
        // Den Bild-Stream öffnen
        using (Stream imageStream = image.GetImageStream(options))
        {
            // Die Datei zum Speichern des Bildes erstellen
            using (Stream destStream = File.Create(Guid.NewGuid().ToString() + ".png"))
            {
                byte[] buffer = new byte[4096];
                int readed = 0;

                do
                {
                    // Daten aus dem Bild-Stream lesen
                    readed = imageStream.Read(buffer, 0, buffer.Length);

                    if (readed > 0)
                    {
                        // Daten in den Datei-Stream schreiben
                        destStream.Write(buffer, 0, readed);
                    }
                }
                while (readed > 0);
            }
        }
    }
}
```

### Siehe auch

* class [ImageOptions](../../../groupdocs.parser.options/imageoptions)
* class [PageImageArea](../../pageimagearea)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->

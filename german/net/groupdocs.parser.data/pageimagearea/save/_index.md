---
title: "Speichern"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Speichert das Bild in die Datei."
type: docs
weight: 50
url: /de/net/groupdocs.parser.data/pageimagearea/save/
---

## Save(string) {#save}

Speichert das Bild in die Datei.

```csharp
public void Save(string filePath)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Der Pfad zur Datei. |

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
        // Speichere das Bild in die Datei
        image.Save(Guid.NewGuid().ToString() + image.FileType.Extension);
    }
}
```

### Siehe auch

* class [PageImageArea](../../pageimagearea)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

---

## Save(string, ImageOptions) {#save_1}

Speichert das Bild in die Datei in einem anderen Format.

```csharp
public void Save(string filePath, ImageOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Der Pfad zur Datei. |
| options | ImageOptions | Die Optionen, die zum Speichern des Bildes verwendet werden. |

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
        // Speichere das Bild in die PNG-Datei
        image.Save(Guid.NewGuid().ToString() + ".png", options);
    }
}
```

### Siehe auch

* class [ImageOptions](../../../groupdocs.parser.options/imageoptions)
* class [PageImageArea](../../pageimagearea)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->

---
title: "GetToc"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Extrahiert ein Inhaltsverzeichnis aus dem Dokument."
type: docs
weight: 200
url: /de/net/groupdocs.parser/parser/gettoc/
---

## Parser.GetToc method

Extrahiert ein Inhaltsverzeichnis aus dem Dokument.

```csharp
public IEnumerable<TocItem> GetToc()
```

### Rückgabewert

Eine Sammlung von Inhaltsverzeichnis‑Elementen; `null`, wenn die Extraktion des Inhaltsverzeichnisses nicht unterstützt wird.

### Hinweise

**Learn more:**

* [Extract table of contents](https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents)
* [Extract text by table of contents item](https://docs.groupdocs.com/display/parsernet/Extract+text+by+table+of+contents+item)
* [Extract table of contents from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents+from+Microsoft+Office+Word+documents)
* [Extract table of contents from EPUB eBooks](https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents+from+EPUB+eBooks)

### Beispiele

Das folgende Beispiel zeigt, wie man das Inhaltsverzeichnis aus einer CHM‑Datei extrahiert:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using (Parser parser = new Parser(filePath))
{
    // Prüfen Sie, ob die Textextraktion unterstützt wird
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }

    // Prüfen, ob die Extraktion des Inhaltsverzeichnisses unterstützt wird
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
 
    // Inhaltsverzeichnis abrufen
    IEnumerable<TocItem> toc = parser.GetToc();
    
    // Über Elemente iterieren
    foreach (TocItem i in toc)
    {
        // Geben Sie den Inhaltsverzeichnistext aus
        Console.WriteLine(i.Text);
        // Prüfen Sie, ob der Seitenindex einen Wert hat
        if (i.PageIndex == null)
        {
            continue;
        }
        // Extrahieren Sie einen Seitentext
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Siehe auch

* class [TocItem](../../../groupdocs.parser.data/tocitem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->

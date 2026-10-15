---
title: "ExtractText"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Extrahiert einen Text aus dem Dokument, auf das das Objekt TocItemgroupdocs.parser.data/tocitem verweist."
type: docs
weight: 50
url: /de/net/groupdocs.parser.data/tocitem/extracttext/
---

## TocItem.ExtractText method

Extrahiert einen Text aus dem Dokument, auf das das Objekt [`TocItem`](../../tocitem) verweist.

```csharp
public virtual TextReader ExtractText()
```

### Rückgabewert

Eine Instanz der TextReader‑Klasse mit dem extrahierten Text.

### Beispiele

Das folgende Beispiel, wie man einen Text über ein Element des Inhaltsverzeichnisses extrahiert:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using (Parser parser = new Parser(Constants.SampleDocxWithToc))
{
    // Inhaltsverzeichnis abrufen
    IEnumerable<TocItem> tocItems = parser.GetToc();
    // Prüfen, ob die Extraktion des Inhaltsverzeichnisses unterstützt wird
    if (tocItems == null)
    {
        Console.WriteLine("Table of contents extraction isn't supported");
    }
    // Über Elemente iterieren
    foreach (TocItem tocItem in tocItems)
    {
        // Den Text des Kapitels ausgeben
        using (TextReader reader = tocItem.ExtractText())
        {
            Console.WriteLine("----");
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Siehe auch

* class [TocItem](../../tocitem)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->

---
title: "GetMetadata"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Extrahiert Metadaten aus dem Dokument."
type: docs
weight: 140
url: /de/net/groupdocs.parser/parser/getmetadata/
---

## Parser.GetMetadata method

Extrahiert Metadaten aus dem Dokument.

```csharp
public IEnumerable<MetadataItem> GetMetadata()
```

### Rückgabewert

Eine Sammlung von Metadaten‑Elementen; `null`, wenn die Metadatenextraktion nicht unterstützt wird.

### Hinweise

**Learn more:**

* [Extract metadata from documents](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+documents)
* [Extract metadata from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+Word+documents)
* [Extract metadata from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+Excel+spreadsheets)
* [Extract metadata from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+PowerPoint+presentations)
* [Extract metadata from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+PDF+documents)
* [Extract metadata from Emails](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Emails)

### Beispiele

Das folgende Beispiel zeigt, wie Metadaten aus einem Dokument extrahiert werden:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using(Parser parser = new Parser(filePath))
{
    // Metadaten aus dem Dokument extrahieren
    IEnumerable<MetadataItem> metadata = parser.GetMetadata();
    // Prüfen, ob die Metadatenextraktion unterstützt wird
    if(metadata == null)
    {
        Console.WriteLine("Metatada extraction isn't supported");
    }
 
    // Durch Metadaten‑Elemente iterieren
    foreach(MetadataItem item in metadata)
    {
        // Den Namen und Wert eines Elements ausgeben
        Console.WriteLine(string.Format("{0}: {1}", item.Name, item.Value));
    }
}
```

### Siehe auch

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->

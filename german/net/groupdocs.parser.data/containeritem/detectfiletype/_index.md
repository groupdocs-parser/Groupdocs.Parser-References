---
title: "DetectFileType"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Erkennt den Dateityp des Container-Elements."
type: docs
weight: 60
url: /de/net/groupdocs.parser.data/containeritem/detectfiletype/
---

## ContainerItem.DetectFileType method

Erkennt den Dateityp des Container-Elements.

```csharp
public FileType DetectFileType(FileTypeDetectionMode detectionMode)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| detectionMode | FileTypeDetectionMode | Definiert einen Modus der Dateityp-Erkennung. |

### Rückgabewert

Eine Instanz der Klasse [`FileType`](../../../groupdocs.parser.options/filetype); [`Unknown`](../../../groupdocs.parser.options/filetype/unknown), wenn kein Dateityp erkannt wird.

### Hinweise

*detectionMode* parameter provides the ability to control file type detection:

* **Default**. The file type is detected by the file extension; if the file extension isn't recognized, the file type is detected by the file content.
* **Extension**.The file type is detected only by the file extension.
* **Content**. The file type is detected only by the file content.

### Beispiele

Das folgende Beispiel zeigt, wie der Dateityp eines Containerelements erkannt wird:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using (Parser parser = new Parser(filePath))
{
    // Anhänge aus dem Container extrahieren
    IEnumerable<ContainerItem> attachments = parser.GetContainer();
    // Prüfen, ob die Container‑Extraktion unterstützt wird
    if (attachments == null)
    {
        Console.WriteLine("Container extraction isn't supported");
    }
    // Durch Anhänge iterieren
    foreach (ContainerItem item in attachments)
    {
        // Den Dateityp erkennen
        Options.FileType fileType = item.DetectFileType(Options.FileTypeDetectionMode.Default);

        // Name und Dateityp ausgeben
        Console.WriteLine(string.Format("{0}: {1}", item.Name, fileType));
    }
}
```

### Siehe auch

* class [FileType](../../../groupdocs.parser.options/filetype)
* enum [FileTypeDetectionMode](../../../groupdocs.parser.options/filetypedetectionmode)
* class [ContainerItem](../../containeritem)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->

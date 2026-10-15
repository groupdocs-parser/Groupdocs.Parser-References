---
title: "GetContainer"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Extrahiert ein Container-Objekt aus dem Dokument, um mit Formaten zu arbeiten, die Anhänge, ZIP-Archive usw. enthalten."
type: docs
weight: 80
url: /de/net/groupdocs.parser/parser/getcontainer/
---

## Parser.GetContainer method

Extrahiert ein Container‑Objekt aus dem Dokument, um mit Formaten zu arbeiten, die Anhänge, ZIP‑Archive usw. enthalten.

```csharp
public IEnumerable<ContainerItem> GetContainer()
```

### Rückgabewert

Eine Sammlung von Container-Elementen; `null`, wenn die Container-Extraktion nicht unterstützt wird.

### Hinweise

Um zu prüfen, ob das Format das Extrahieren von Anhängen unterstützt, siehe [Supported Document Formats](https://docs.groupdocs.com/parser/net/supported-document-formats/) (**Extract Containers and Attachments** Spalte).

**Learn more:**

* [Extract data from attachments and ZIP archives](https://docs.groupdocs.com/display/parsernet/Extract+data+from+attachments+and+ZIP+archives)
* [Iterate through container items](https://docs.groupdocs.com/display/parsernet/Iterate+through+container+items)
* [Extract attachments from PDF portfolios](https://docs.groupdocs.com/display/parsernet/Extract+attachments+from+PDF+portfolios)
* [Extract attachments from Emails](https://docs.groupdocs.com/display/parsernet/Extract+attachments+from+Emails)
* [Extract emails from Outlook Storage](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+Outlook+Storage)
* [Extract text from ZIP archive files](https://docs.groupdocs.com/display/parsernet/Extract+text+from+ZIP+archive+files)

### Beispiele

Das folgende Beispiel zeigt, wie Anhänge aus einem Container extrahiert werden:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using(Parser parser = new Parser(filePath))
{
    // Anhänge aus dem Container extrahieren
    IEnumerable<ContainerItem> attachments = parser.GetContainer();
    // Prüfen, ob die Container‑Extraktion unterstützt wird
    if(attachments == null)
    {
        Console.WriteLine("Container extraction isn't supported");
    }
 
    // Durch Anhänge iterieren
    foreach(ContainerItem item in attachments)
    {
        // Gibt den Namen und die Größe eines Elements aus
        Console.WriteLine(string.Format("{0}: {1}", item.Name, item.Size));
    }
}
```

### Siehe auch

* class [ContainerItem](../../../groupdocs.parser.data/containeritem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->

---
title: "ParseForm"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Parst das Dokumentformular."
type: docs
weight: 240
url: /de/net/groupdocs.parser/parser/parseform/
---

## Parser.ParseForm method

Parst das Dokumentformular.

```csharp
public DocumentData ParseForm()
```

### Rückgabewert

Eine Instanz der [`DocumentData`](../../../groupdocs.parser.data/documentdata)-Klasse, die die extrahierten Daten enthält; `null`, wenn das Parsen anhand einer Vorlage nicht unterstützt wird.

### Hinweise

**Learn more:**

* [Extract data from PDF forms](https://docs.groupdocs.com/display/parsernet/Extract+data+from+PDF+forms)
* [Working with extracted data](https://docs.groupdocs.com/display/parsernet/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+PDF+documents)

### Beispiele

Das folgende Beispiel zeigt, wie ein Formular des Dokuments geparst wird:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using (Parser parser = new Parser(filePath))
{
    // Daten aus PDF-Dokument extrahieren
    DocumentData data = parser.ParseForm();
    // Iterieren über extrahierte Daten
    for (int i = 0; i<data.Count; i++)
    {
        Console.Write(data[i].Name + ": ");
        PageTextArea area = data[i].PageArea as PageTextArea;
        Console.WriteLine(area == null ? "Not a template field" : area.Text);
    }
}
```

### Siehe auch

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->

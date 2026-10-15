---
title: "GetDocumentInfo"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Gibt die allgemeinen Informationen zum Dokument zurück."
type: docs
weight: 90
url: /de/net/groupdocs.parser/parser/getdocumentinfo/
---

## Parser.GetDocumentInfo method

Gibt die allgemeinen Informationen zum Dokument zurück.

```csharp
public IDocumentInfo GetDocumentInfo()
```

### Rückgabewert

Eine Instanz einer Klasse, die das Interface [`IDocumentInfo`](../../../groupdocs.parser.options/idocumentinfo) implementiert.

### Hinweise

**Learn more:**

* [Get document info](https://docs.groupdocs.com/display/parsernet/Get+document+info)
* [Detect encoding](https://docs.groupdocs.com/display/parsernet/Detect+encoding)

### Beispiele

Das folgende Beispiel zeigt, wie man Dokumentinformationen abruft:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using(Parser parser = new Parser(filePath))
{
    // Rufe die Dokumentinformationen ab
    IDocumentInfo info = parser.GetDocumentInfo();

    Console.WriteLine(string.Format("FileType: {0}", info.FileType));
    Console.WriteLine(string.Format("PageCount: {0}", info.PageCount));
    Console.WriteLine(string.Format("Size: {0}", info.Size));
}
```

### Siehe auch

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->

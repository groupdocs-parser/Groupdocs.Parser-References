---
title: "GetHighlight"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Extrahiert eine Hervorhebung aus dem Dokument."
type: docs
weight: 110
url: /de/net/groupdocs.parser/parser/gethighlight/
---

## Parser.GetHighlight method

Extrahiert eine Hervorhebung aus dem Dokument.

```csharp
public HighlightItem GetHighlight(int position, bool isDirect, HighlightOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Position | Int32 | Die Startposition der Hervorhebung. |
| isDirect | Boolean | Der Wert, der angibt, ob die Hervorhebungsextraktion direkt ist. `true`, wenn die Hervorhebung rechts von *position* extrahiert wird; andernfalls `false`. |
| options | HighlightOptions | Die Optionen für die Hervorhebungsextraktion. |

### Rückgabewert

Eine Instanz der Klasse [`HighlightItem`](../../../groupdocs.parser.data/highlightitem), die die extrahierte Hervorhebung darstellt; `null`, wenn die Hervorhebungsextraktion nicht unterstützt wird.

### Hinweise

**Learn more:**

* [Extract highlights](https://docs.groupdocs.com/display/parsernet/Extract+highlights)

### Beispiele

Das folgende Beispiel zeigt, wie eine Hervorhebung extrahiert wird, die 3 Wörter enthält:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using (Parser parser = new Parser(filePath))
{
    // Hervorhebung extrahieren:
    HighlightItem hl = parser.GetHighlight(2, true, new HighlightOptions(3));
    
    // Prüfen, ob die Hervorhebungsextraktion unterstützt wird
    if (hl == null)
    {
        Console.WriteLine("Highlight extraction isn't supported");
        return;
    }
    
    // Eine extrahierte Hervorhebung ausgeben
    Console.WriteLine(string.Format("At {0}: {1}", hl.Position, hl.Text));
}
```

### Siehe auch

* class [HighlightItem](../../../groupdocs.parser.data/highlightitem)
* class [HighlightOptions](../../../groupdocs.parser.options/highlightoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->

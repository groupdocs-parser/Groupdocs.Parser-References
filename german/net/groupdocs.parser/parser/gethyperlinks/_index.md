---
title: GetHyperlinks
second_title: GroupDocs.Parser für .NET-API-Referenz
description: Extrahiert Hyperlinks aus dem Dokument.
type: docs
weight: 100
url: /de/net/groupdocs.parser/parser/gethyperlinks/
---
## GetHyperlinks() {#gethyperlinks}

Extrahiert Hyperlinks aus dem Dokument.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks()
```

### Rückgabewert

Eine Sammlung von[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) Objekte; `Null` wenn das Extrahieren von Hyperlinks nicht unterstützt wird.

### Beispiele

Das folgende Beispiel zeigt, wie alle Hyperlinks aus dem gesamten Dokument extrahiert werden:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse
using (Parser parser = new Parser(filePath))
{
    // Prüfen Sie, ob das Dokument die Extraktion von Hyperlinks unterstützt
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Hyperlinks aus dem Dokument extrahieren
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks();
    // Über Hyperlinks iterieren
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Den Text des Hyperlinks drucken
        Console.WriteLine(h.Text);
        // Hyperlink-URL drucken
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Siehe auch

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int) {#gethyperlinks_2}

Extrahiert Hyperlinks von der Dokumentseite.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | Int32 | Der nullbasierte Seitenindex. |

### Rückgabewert

Eine Sammlung von[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) Objekte; `Null` wenn das Extrahieren von Hyperlinks nicht unterstützt wird.

### Beispiele

Das folgende Beispiel zeigt, wie Hyperlinks aus der Dokumentseite extrahiert werden:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse
using (Parser parser = new Parser(filePath))
{
    // Prüfen Sie, ob das Dokument die Extraktion von Hyperlinks unterstützt
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Holen Sie sich die Dokumentinformationen
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Prüfe, ob das Dokument Seiten hat
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    // Über Seiten iterieren
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Eine Seitenzahl drucken 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Hyperlinks von der Dokumentseite extrahieren
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex);
        // Über Hyperlinks iterieren
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Den Text des Hyperlinks drucken
            Console.WriteLine(h.Text);
            // Hyperlink-URL drucken
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
    }
}
```

### Siehe auch

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## GetHyperlinks(PageAreaOptions) {#gethyperlinks_1}

Extrahiert Hyperlinks aus dem Dokument mithilfe von Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Hyperlinks enthält).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(PageAreaOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | PageAreaOptions | Die Optionen zum Extrahieren von Hyperlinks. |

### Rückgabewert

Eine Sammlung von[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) Objekte; `Null` wenn das Extrahieren von Hyperlinks nicht unterstützt wird.

### Beispiele

Das folgende Beispiel zeigt, wie Hyperlinks aus dem Dokumentseitenbereich extrahiert werden:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse
using (Parser parser = new Parser(filePath))
{
    // Prüfen Sie, ob das Dokument die Extraktion von Hyperlinks unterstützt
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Erstellen Sie die Optionen, die für die Hyperlink-Extraktion verwendet werden
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Hyperlinks aus dem Seitenbereich des Dokuments extrahieren
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(options);
    // Über Hyperlinks iterieren
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Den Text des Hyperlinks drucken
        Console.WriteLine(h.Text);
        // Hyperlink-URL drucken
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Siehe auch

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int, PageAreaOptions) {#gethyperlinks_3}

Extrahiert Hyperlinks von der Dokumentseite mithilfe von Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Hyperlinks enthält).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex, PageAreaOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | Int32 | Der nullbasierte Seitenindex. |
| options | PageAreaOptions | Die Optionen zum Extrahieren von Hyperlinks. |

### Rückgabewert

Eine Sammlung von[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) Objekte; `Null` wenn das Extrahieren von Hyperlinks nicht unterstützt wird.

### Beispiele

Das folgende Beispiel zeigt, wie Sie mithilfe von Anpassungsoptionen Hyperlinks aus dem Dokumentseitenbereich extrahieren:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse
using (Parser parser = new Parser(filePath))
{
    // Prüfen Sie, ob das Dokument die Extraktion von Hyperlinks unterstützt
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    
    // Holen Sie sich die Dokumentinformationen
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Prüfe, ob das Dokument Seiten hat
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // Erstellen Sie die Optionen, die für die Hyperlink-Extraktion verwendet werden
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Über Seiten iterieren
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Eine Seitenzahl drucken 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));         
        // Hyperlinks aus dem Seitenbereich des Dokuments extrahieren
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex, options);
        // Über Hyperlinks iterieren
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Den Text des Hyperlinks drucken
            Console.WriteLine(h.Text);
            // Hyperlink-URL drucken
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
}
```

### Siehe auch

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

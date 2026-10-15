---
title: "GetHyperlinks"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Extrahiert Hyperlinks aus dem Dokument."
type: docs
weight: 120
url: /de/net/groupdocs.parser/parser/gethyperlinks/
---

## GetHyperlinks() {#gethyperlinks}

Extrahiert Hyperlinks aus dem Dokument.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks()
```

### Rückgabewert

Eine Sammlung von [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea)-Objekten; `null`, wenn die Hyperlink-Extraktion nicht unterstützt wird.

### Beispiele

Das folgende Beispiel zeigt, wie man alle Hyperlinks aus dem gesamten Dokument extrahiert:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using (Parser parser = new Parser(filePath))
{
    // Prüfen Sie, ob das Dokument die Hyperlink-Extraktion unterstützt
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Extrahieren Sie Hyperlinks aus dem Dokument
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks();
    // Iterieren Sie über Hyperlinks
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Geben Sie den Hyperlink-Text aus
        Console.WriteLine(h.Text);
        // Geben Sie die Hyperlink-URL aus
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Siehe auch

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int) {#gethyperlinks_2}

Extrahiert Hyperlinks aus der Dokumentseite.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | Int32 | Der nullbasierte Seitenindex. |

### Rückgabewert

Eine Sammlung von [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea)-Objekten; `null`, wenn die Hyperlink-Extraktion nicht unterstützt wird.

### Beispiele

Das folgende Beispiel zeigt, wie man Hyperlinks aus der Dokumentseite extrahiert:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using (Parser parser = new Parser(filePath))
{
    // Prüfen Sie, ob das Dokument die Hyperlink-Extraktion unterstützt
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Rufe die Dokumentinformationen ab
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Prüfe, ob das Dokument Seiten hat
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    // Iteriere über die Seiten
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Gib eine Seitenzahl aus 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Extrahieren Sie Hyperlinks aus der Dokumentseite
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex);
        // Iterieren Sie über Hyperlinks
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Geben Sie den Hyperlink-Text aus
            Console.WriteLine(h.Text);
            // Geben Sie die Hyperlink-URL aus
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
    }
}
```

### Siehe auch

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(PageAreaOptions) {#gethyperlinks_1}

Extrahiert Hyperlinks aus dem Dokument mithilfe von Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Hyperlinks enthält).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(PageAreaOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | PageAreaOptions | Die Optionen für die Hyperlink-Extraktion. |

### Rückgabewert

Eine Sammlung von [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea)-Objekten; `null`, wenn die Hyperlink-Extraktion nicht unterstützt wird.

### Beispiele

Das folgende Beispiel zeigt, wie man Hyperlinks aus dem Dokumentseitenbereich extrahiert:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using (Parser parser = new Parser(filePath))
{
    // Prüfen Sie, ob das Dokument die Hyperlink-Extraktion unterstützt
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Erstellen Sie die Optionen, die für die Hyperlink-Extraktion verwendet werden
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Extrahieren Sie Hyperlinks aus dem Dokumentseitenbereich
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(options);
    // Iterieren Sie über Hyperlinks
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Geben Sie den Hyperlink-Text aus
        Console.WriteLine(h.Text);
        // Geben Sie die Hyperlink-URL aus
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Siehe auch

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int, PageAreaOptions) {#gethyperlinks_3}

Extrahiert Hyperlinks aus der Dokumentseite mithilfe von Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Hyperlinks enthält).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex, PageAreaOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | Int32 | Der nullbasierte Seitenindex. |
| options | PageAreaOptions | Die Optionen für die Hyperlink-Extraktion. |

### Rückgabewert

Eine Sammlung von [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea)-Objekten; `null`, wenn die Hyperlink-Extraktion nicht unterstützt wird.

### Beispiele

Das folgende Beispiel zeigt, wie man Hyperlinks aus dem Dokumentseitenbereich mithilfe von Anpassungsoptionen extrahiert:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using (Parser parser = new Parser(filePath))
{
    // Prüfen Sie, ob das Dokument die Hyperlink-Extraktion unterstützt
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    
    // Rufe die Dokumentinformationen ab
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Prüfe, ob das Dokument Seiten hat
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // Erstellen Sie die Optionen, die für die Hyperlink-Extraktion verwendet werden
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Iteriere über die Seiten
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Gib eine Seitenzahl aus 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));         
        // Extrahieren Sie Hyperlinks aus dem Dokumentseitenbereich
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex, options);
        // Iterieren Sie über Hyperlinks
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Geben Sie den Hyperlink-Text aus
            Console.WriteLine(h.Text);
            // Geben Sie die Hyperlink-URL aus
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
}
```

### Siehe auch

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->

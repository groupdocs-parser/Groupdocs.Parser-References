---
title: GetTextAreas
second_title: GroupDocs.Parser für .NET-API-Referenz
description: Extrahiert Textbereiche aus dem Dokument.
type: docs
weight: 160
url: /de/net/groupdocs.parser/parser/gettextareas/
---
## GetTextAreas() {#gettextareas}

Extrahiert Textbereiche aus dem Dokument.

```csharp
public IEnumerable<PageTextArea> GetTextAreas()
```

### Rückgabewert

Eine Sammlung von[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) Objekte; `Null` wenn die Extraktion von Textbereichen nicht unterstützt wird.

### Bemerkungen

**Mehr erfahren:**

* [Textbereiche extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Beispiele

Das folgende Beispiel zeigt, wie Sie alle Textbereiche aus dem gesamten Dokument extrahieren:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse
using(Parser parser = new Parser(filePath))
{
    // Textbereiche extrahieren
    IEnumerable<PageTextArea> areas = parser.GetTextAreas();
    // Prüfen Sie, ob die Extraktion von Textbereichen unterstützt wird
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Seitentextbereiche durchlaufen
    foreach(PageTextArea a in areas)
    {
        // Drucken Sie einen Seitenindex, ein Rechteck und einen Textbereichswert:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Siehe auch

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## GetTextAreas(PageTextAreaOptions) {#gettextareas_1}

Extrahiert Textbereiche aus dem Dokument mithilfe von Anpassungsoptionen (regulärer Ausdruck, Groß-/Kleinschreibung usw.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(PageTextAreaOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | PageTextAreaOptions | Die Optionen für die Textbereichsextraktion. |

### Rückgabewert

Eine Sammlung von[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) Objekte; `Null` wenn die Extraktion von Textbereichen nicht unterstützt wird.

### Bemerkungen

**Mehr erfahren:**

* [Textbereiche extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Beispiele

Das folgende Beispiel zeigt, wie nur Textbereiche mit Ziffern aus der oberen linken Ecke extrahiert werden:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse
using(Parser parser = new Parser(filePath))
{
    // Erstellen Sie die Optionen, die für die Textbereichsextraktion verwendet werden
    PageTextAreaOptions options = new PageTextAreaOptions("[0-9]+", new Rectangle(new Point(0, 0), new Size(300, 100)));

    // Textbereiche extrahieren, die nur Ziffern aus der oberen linken Ecke einer Seite enthalten:
    IEnumerable<PageTextArea> areas = parser.GetTextAreas(options);
    // Prüfen Sie, ob die Extraktion von Textbereichen unterstützt wird
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Seitentextbereiche durchlaufen
    foreach(PageTextArea a in areas)
    {
        // Drucken Sie einen Seitenindex, ein Rechteck und einen Textbereichswert:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Siehe auch

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## GetTextAreas(int) {#gettextareas_2}

Extrahiert Textbereiche aus der Dokumentseite.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | Int32 | Der nullbasierte Seitenindex. |

### Rückgabewert

Eine Sammlung von[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) Objekte; `Null` wenn die Extraktion von Textbereichen nicht unterstützt wird.

### Bemerkungen

**Mehr erfahren:**

* [Textbereiche extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Beispiele

Um Textbereiche aus einer Dokumentseite zu extrahieren, wird die folgende Methode verwendet:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse
using(Parser parser = new Parser(filePath))
{
    // Prüfen, ob das Dokument die Extraktion von Textbereichen unterstützt
    if(!parser.Features.TextAreas)
    {
        Console.WriteLine("Document isn't supports text areas extraction.");
        return;
    }

    // Holen Sie sich die Dokumentinformationen
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Prüfe, ob das Dokument Seiten hat
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Über Seiten iterieren
    for(int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Eine Seitenzahl drucken 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
 
        // Seitentextbereiche durchlaufen
        // Wir ignorieren die Nullprüfung, da wir zuvor die Unterstützung der Textbereichsextraktionsfunktion überprüft haben
        foreach(PageTextArea a in parser.GetTextAreas(pageIndex))
        {
            // Einen Rechteck- und Textbereichswert drucken:
            Console.WriteLine(string.Format("R: {0}, Text: {1}", a.Rectangle, a.Text));
        }
    }
}
```

### Siehe auch

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## GetTextAreas(int, PageTextAreaOptions) {#gettextareas_3}

Extrahiert Textbereiche aus der Dokumentseite mithilfe von Anpassungsoptionen (regulärer Ausdruck, Groß-/Kleinschreibung usw.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex, PageTextAreaOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | Int32 | Der nullbasierte Seitenindex. |
| options | PageTextAreaOptions | Die Optionen für die Textbereichsextraktion. |

### Rückgabewert

Eine Sammlung von[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) Objekte; `Null` wenn die Extraktion von Textbereichen nicht unterstützt wird.

### Bemerkungen

**Mehr erfahren:**

* [Textbereiche extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Siehe auch

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

---
title: GetImages
second_title: GroupDocs.Parser für .NET-API-Referenz
description: Extrahiert Bilder aus dem Dokument.
type: docs
weight: 110
url: /de/net/groupdocs.parser/parser/getimages/
---
## GetImages() {#getimages}

Extrahiert Bilder aus dem Dokument.

```csharp
public IEnumerable<PageImageArea> GetImages()
```

### Rückgabewert

Eine Sammlung von[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) Objekte; `Null` wenn die Bildextraktion nicht unterstützt wird.

### Bemerkungen

**Erfahren Sie mehr:**

* [Bilder aus Dokumenten extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Bilder in Dateien extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extrahieren Sie Bilder aus Microsoft Office Word-Dokumenten](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extrahieren Sie Bilder aus Microsoft Office Excel-Tabellen](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extrahieren Sie Bilder aus Microsoft Office PowerPoint-Präsentationen](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Bilder aus E-Mails extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Bilder aus PDF-Dokumenten extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Beispiele

Das folgende Beispiel zeigt, wie alle Bilder aus dem gesamten Dokument extrahiert werden:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse
using (Parser parser = new Parser(filePath))
{
    // Bilder extrahieren
    IEnumerable<PageImageArea> images = parser.GetImages();
    // Prüfen Sie, ob die Extraktion von Bildern unterstützt wird
    if (images == null)
    {
        Console.WriteLine("Images extraction isn't supported");
        return;
    }
    // Über Bilder iterieren
    foreach (PageImageArea image in images)
    {
        // Seitenindex, Rechteck und Bildtyp drucken:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Siehe auch

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## GetImages(PageAreaOptions) {#getimages_1}

Extrahiert Bilder aus dem Dokument mithilfe der Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Bilder enthält).

```csharp
public IEnumerable<PageImageArea> GetImages(PageAreaOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | PageAreaOptions | Die Optionen für die Bildextraktion. |

### Rückgabewert

Eine Sammlung von[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) Objekte; `Null` wenn die Bildextraktion nicht unterstützt wird.

### Bemerkungen

**Erfahren Sie mehr:**

* [Bilder aus Dokumenten extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Bilder in Dateien extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extrahieren Sie Bilder aus dem Dokumentseitenbereich](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extrahieren Sie Bilder aus Microsoft Office Word-Dokumenten](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extrahieren Sie Bilder aus Microsoft Office Excel-Tabellen](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extrahieren Sie Bilder aus Microsoft Office PowerPoint-Präsentationen](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Bilder aus E-Mails extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Bilder aus PDF-Dokumenten extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Beispiele

Das folgende Beispiel zeigt, wie Sie nur Bilder aus der oberen linken Ecke extrahieren:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse
using (Parser parser = new Parser(filePath))
{
    // Erstellen Sie die Optionen, die für die Bildextraktion verwendet werden
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(0, 0), new Size(300, 100)));
    // Bilder aus der oberen linken Ecke einer Seite extrahieren:
    IEnumerable<PageImageArea> images = parser.GetImages(options);
    // Prüfen Sie, ob die Extraktion von Bildern unterstützt wird
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }
    // Über Bilder iterieren
    foreach (PageImageArea image in images)
    {
        // Seitenindex, Rechteck und Bildtyp drucken:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Siehe auch

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## GetImages(int) {#getimages_2}

Extrahiert Bilder von der Dokumentseite.

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | Int32 | Der nullbasierte Seitenindex. |

### Rückgabewert

Eine Sammlung von[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) Objekte; `Null` wenn die Bildextraktion nicht unterstützt wird.

### Bemerkungen

**Erfahren Sie mehr:**

* [Bilder aus Dokumenten extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Bilder in Dateien extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extrahieren Sie Bilder von der Dokumentseite](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extrahieren Sie Bilder aus Microsoft Office Word-Dokumenten](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extrahieren Sie Bilder aus Microsoft Office Excel-Tabellen](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extrahieren Sie Bilder aus Microsoft Office PowerPoint-Präsentationen](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Bilder aus E-Mails extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Bilder aus PDF-Dokumenten extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Beispiele

Um Bilder aus einer Dokumentseite zu extrahieren, wird die folgende Methode verwendet:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse
using (Parser parser = new Parser(filePath))
{
    // Prüfen Sie, ob das Dokument die Extraktion von Bildern unterstützt
    if (!parser.Features.Images)
    {
        Console.WriteLine("Document isn't supports images extraction.");
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
    for (int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Eine Seitenzahl drucken 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Über Bilder iterieren
        // Wir ignorieren die Nullprüfung, da wir die Unterstützung der Bildextraktionsfunktion früher überprüft haben
        foreach (PageImageArea image in parser.GetImages(pageIndex))
        {
            // Drucken Sie ein Rechteck und einen Bildtyp
            Console.WriteLine(string.Format("R: {0}, Text: {1}", image.Rectangle, image.FileType));
        }
    }
}
```

### Siehe auch

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## GetImages(int, PageAreaOptions) {#getimages_3}

Extrahiert Bilder von der Dokumentseite mit Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Bilder enthält).

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex, PageAreaOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | Int32 | Der nullbasierte Seitenindex. |
| options | PageAreaOptions | Die Optionen für die Bildextraktion. |

### Rückgabewert

Eine Sammlung von[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) Objekte; `Null` wenn die Bildextraktion nicht unterstützt wird.

### Bemerkungen

**Erfahren Sie mehr:**

* [Bilder aus Dokumenten extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Bilder in Dateien extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extrahieren Sie Bilder von der Dokumentseite](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extrahieren Sie Bilder aus dem Dokumentseitenbereich](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extrahieren Sie Bilder aus Microsoft Office Word-Dokumenten](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extrahieren Sie Bilder aus Microsoft Office Excel-Tabellen](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extrahieren Sie Bilder aus Microsoft Office PowerPoint-Präsentationen](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Bilder aus E-Mails extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Bilder aus PDF-Dokumenten extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Siehe auch

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

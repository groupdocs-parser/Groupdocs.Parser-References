---
title: GetFormattedText
second_title: GroupDocs.Parser für .NET-API-Referenz
description: Extrahiert einen formatierten Text aus dem Dokument.
type: docs
weight: 80
url: /de/net/groupdocs.parser/parser/getformattedtext/
---
## GetFormattedText(FormattedTextOptions) {#getformattedtext}

Extrahiert einen formatierten Text aus dem Dokument.

```csharp
public TextReader GetFormattedText(FormattedTextOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | FormattedTextOptions | Die Extraktionsoptionen für formatierten Text. |

### Rückgabewert

Eine Instanz vonTextReader Klasse mit dem extrahierten Text; `Null` wenn die Extraktion von formatiertem Text nicht unterstützt wird.

### Bemerkungen

**Mehr erfahren:**

* [Formatierten Text aus Dokument extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+formatted+text+from+document)
* Extrahieren Sie einen Dokumenttext als[HTML](https://docs.groupdocs.com/display/parsernet/HTML)
* Extrahieren Sie einen Dokumenttext als[Abschlag](https://docs.groupdocs.com/display/parsernet/Markdown)
* Extrahieren Sie einen Dokumenttext als[Klartext](https://docs.groupdocs.com/display/parsernet/Plain+text)

### Beispiele

Das folgende Beispiel zeigt, wie Sie einen Dokumenttext als HTML-Text extrahieren:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse
using (Parser parser = new Parser(filePath))
{
    // Einen formatierten Text in den Reader extrahieren
    using (TextReader reader = parser.GetFormattedText(new FormattedTextOptions(FormattedTextMode.Html)))
    {
        // Einen formatierten Text aus dem Dokument drucken
        // Wenn die Extraktion von formatiertem Text nicht unterstützt wird, ist ein Reader null
        Console.WriteLine(reader == null ? "Formatted text extraction isn't suppported" : reader.ReadToEnd());
    }
}
```

### Siehe auch

* class [FormattedTextOptions](../../../groupdocs.parser.options/formattedtextoptions)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## GetFormattedText(int, FormattedTextOptions) {#getformattedtext_1}

Extrahiert einen formatierten Text aus der Dokumentseite.

```csharp
public TextReader GetFormattedText(int pageIndex, FormattedTextOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | Int32 | Der nullbasierte Seitenindex. |
| options | FormattedTextOptions | Die Extraktionsoptionen für formatierten Text. |

### Rückgabewert

Eine Instanz vonTextReaderKlasse mit dem extrahierten Text; `Null` wenn die Extraktion formatierter Textseiten nicht unterstützt wird.

### Bemerkungen

**Mehr erfahren:**

* [Extrahieren Sie formatierten Text von der Dokumentseite](https://docs.groupdocs.com/display/parsernet/Extract+formatted+text+from+document+page)
* Extrahieren Sie einen Dokumenttext als[HTML](https://docs.groupdocs.com/display/parsernet/HTML)
* Extrahieren Sie einen Dokumenttext als[Abschlag](https://docs.groupdocs.com/display/parsernet/Markdown)
* Extrahieren Sie einen Dokumenttext als[Klartext](https://docs.groupdocs.com/display/parsernet/Plain+text)

### Beispiele

Das folgende Beispiel zeigt, wie Sie einen Dokumentseitentext als Markdown-Text extrahieren:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse
using (Parser parser = new Parser(filePath))
{
    // Prüfen Sie, ob das Dokument die Extraktion von formatiertem Text unterstützt
    if (!parser.Features.FormattedText)
    {
        Console.WriteLine("Document isn't supports formatted text extraction.");
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
    for (int p = 0; p<documentInfo.PageCount; p++)
    {
        // Eine Seitenzahl drucken 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
        // Einen formatierten Text in den Reader extrahieren
        using (TextReader reader = parser.GetFormattedText(p, new FormattedTextOptions(FormattedTextMode.Markdown)))
        {
            // Einen formatierten Text aus dem Dokument drucken
            // Wir ignorieren die Nullprüfung, da wir zuvor die Unterstützung für formatierte Textextraktionsfunktionen überprüft haben
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Siehe auch

* class [FormattedTextOptions](../../../groupdocs.parser.options/formattedtextoptions)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
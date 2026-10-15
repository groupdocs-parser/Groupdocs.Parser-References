---
title: "GetFormattedText"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Extrahiert einen formatierten Text aus dem Dokument."
type: docs
weight: 100
url: /de/net/groupdocs.parser/parser/getformattedtext/
---

## GetFormattedText(FormattedTextOptions) {#getformattedtext}

Extrahiert einen formatierten Text aus dem Dokument.

```csharp
public TextReader GetFormattedText(FormattedTextOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | FormattedTextOptions | Die Optionen für die formatierte Textextraktion. |

### Rückgabewert

Eine Instanz der TextReader-Klasse mit dem extrahierten Text; `null`, wenn die formatierte Textextraktion nicht unterstützt wird.

### Hinweise

**Learn more:**

* [Extract formatted text from document](https://docs.groupdocs.com/display/parsernet/Extract+formatted+text+from+document)
* Extract a document text as [HTML](https://docs.groupdocs.com/display/parsernet/HTML)
* Extract a document text as [Markdown](https://docs.groupdocs.com/display/parsernet/Markdown)
* Extract a document text as [Plain text](https://docs.groupdocs.com/display/parsernet/Plain+text)

### Beispiele

Das folgende Beispiel zeigt, wie man den Dokumententext als HTML-Text extrahiert:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using (Parser parser = new Parser(filePath))
{
    // Extrahiere einen formatierten Text in den Reader
    using (TextReader reader = parser.GetFormattedText(new FormattedTextOptions(FormattedTextMode.Html)))
    {
        // Formatierten Text aus dem Dokument ausgeben
        // Wenn die Extraktion formatierten Textes nicht unterstützt wird, ist ein Reader null
        Console.WriteLine(reader == null ? "Formatted text extraction isn't suppported" : reader.ReadToEnd());
    }
}
```

### Siehe auch

* class [FormattedTextOptions](../../../groupdocs.parser.options/formattedtextoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetFormattedText(int, FormattedTextOptions) {#getformattedtext_1}

Extrahiert einen formatierten Text aus der Dokumentseite.

```csharp
public TextReader GetFormattedText(int pageIndex, FormattedTextOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | Int32 | Der nullbasierte Seitenindex. |
| options | FormattedTextOptions | Die Optionen für die formatierte Textextraktion. |

### Rückgabewert

Eine Instanz der TextReader-Klasse mit dem extrahierten Text; `null`, wenn die Extraktion formatierter Textseiten nicht unterstützt wird.

### Hinweise

**Learn more:**

* [Extract formatted text from document page](https://docs.groupdocs.com/display/parsernet/Extract+formatted+text+from+document+page)
* Extract a document text as [HTML](https://docs.groupdocs.com/display/parsernet/HTML)
* Extract a document text as [Markdown](https://docs.groupdocs.com/display/parsernet/Markdown)
* Extract a document text as [Plain text](https://docs.groupdocs.com/display/parsernet/Plain+text)

### Beispiele

Das folgende Beispiel zeigt, wie man den Text einer Dokumentseite als Markdown-Text extrahiert:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using (Parser parser = new Parser(filePath))
{
    // Überprüfen, ob das Dokument die Extraktion formatierten Textes unterstützt
    if (!parser.Features.FormattedText)
    {
        Console.WriteLine("Document isn't supports formatted text extraction.");
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
    for (int p = 0; p<documentInfo.PageCount; p++)
    {
        // Gib eine Seitenzahl aus 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
        // Extrahiere einen formatierten Text in den Reader
        using (TextReader reader = parser.GetFormattedText(p, new FormattedTextOptions(FormattedTextMode.Markdown)))
        {
            // Formatierten Text aus dem Dokument ausgeben
            // Wir ignorieren die Nullprüfung, da wir die Unterstützung der Extraktion formatierten Textes bereits vorher geprüft haben
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Siehe auch

* class [FormattedTextOptions](../../../groupdocs.parser.options/formattedtextoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->

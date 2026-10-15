---
title: "GetText"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Extrahiert einen Text aus dem Dokument."
type: docs
weight: 180
url: /de/net/groupdocs.parser/parser/gettext/
---

## GetText() {#gettext}

Extrahiert einen Text aus dem Dokument.

```csharp
public TextReader GetText()
```

### Rückgabewert

Eine Instanz der Klasse TextReader mit dem extrahierten Text; `null`, wenn die Textextraktion nicht unterstützt wird.

### Hinweise

**Learn more:**

* [Extract text from documents](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Beispiele

Das folgende Beispiel zeigt, wie ein Text aus einem Dokument extrahiert wird:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using(Parser parser = new Parser(filePath))
{
    // Text in den Reader extrahieren
    using(TextReader reader = parser.GetText())
    {
        // Text aus dem Dokument ausgeben
        // Wenn die Textextraktion nicht unterstützt wird, ist ein Reader null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Siehe auch

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(TextOptions) {#gettext_1}

Extrahiert eine Textseite aus dem Dokument mithilfe von Textoptionen (um den Roh‑Schnelltextextraktionsmodus zu aktivieren).

```csharp
public TextReader GetText(TextOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | TextOptions | Die Optionen für die Textextraktion. |

### Rückgabewert

Eine Instanz der Klasse TextReader mit dem extrahierten Text; `null`, wenn die Textextraktion nicht unterstützt wird.

### Hinweise

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Beispiele

Das folgende Beispiel zeigt, wie ein Rohtext aus einem Dokument extrahiert wird:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using(Parser parser = new Parser(filePath))
{
    // Extrahiere einen Rohtext in den Reader
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // Text aus dem Dokument ausgeben
        // Wenn die Textextraktion nicht unterstützt wird, ist ein Reader null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Siehe auch

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

Extrahiert einen Text aus der Dokumentseite.

```csharp
public TextReader GetText(int pageIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | Int32 | Der nullbasierte Seitenindex. |

### Rückgabewert

Eine Instanz der TextReader-Klasse mit dem extrahierten Text; `null`, wenn die Extraktion von Textseiten nicht unterstützt wird.

### Hinweise

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Beispiele

Das folgende Beispiel zeigt, wie man einen Text aus der Dokumentenseite extrahiert:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using(Parser parser = new Parser(filePath))
{
    // Prüfe, ob das Dokument die Textextraktion unterstützt
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Rufe die Dokumentinformationen ab
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Prüfe, ob das Dokument Seiten hat
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Iteriere über die Seiten
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // Gib eine Seitenzahl aus 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // Text in den Reader extrahieren
        using(TextReader reader = parser.GetText(p))
        {
            // Text aus dem Dokument ausgeben
            // Wir ignorieren die Nullprüfung, da wir die Unterstützung der Textextraktionsfunktion bereits vorher geprüft haben
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Siehe auch

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(int, TextOptions) {#gettext_3}

Extrahiert einen Text aus der Dokumentseite mithilfe von Textoptionen (um den Roh‑Schnelltextextraktionsmodus zu aktivieren).

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | Int32 | Der nullbasierte Seitenindex. |
| options | TextOptions | Die Optionen für die Textextraktion. |

### Rückgabewert

Eine Instanz der TextReader-Klasse mit dem extrahierten Text; `null`, wenn die Extraktion von Textseiten nicht unterstützt wird.

### Hinweise

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Beispiele

Das folgende Beispiel zeigt, wie man einen Rohtext aus der Dokumentenseite extrahiert:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using(Parser parser = new Parser(filePath))
{
    // Prüfe, ob das Dokument die Textextraktion unterstützt
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Rufe die Dokumentinformationen ab
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // Prüfe, ob das Dokument Seiten hat
    if(documentInfo == null || documentInfo.RawPageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Iteriere über die Seiten
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // Gib eine Seitenzahl aus 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // Text in den Reader extrahieren
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // Text aus dem Dokument ausgeben
            // Wir ignorieren die Nullprüfung, da wir die Unterstützung der Textextraktionsfunktion bereits vorher geprüft haben
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Siehe auch

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->

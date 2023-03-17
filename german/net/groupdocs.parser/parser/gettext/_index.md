---
title: GetText
second_title: GroupDocs.Parser für .NET-API-Referenz
description: Extrahiert einen Text aus dem Dokument.
type: docs
weight: 150
url: /de/net/groupdocs.parser/parser/gettext/
---
## GetText() {#gettext}

Extrahiert einen Text aus dem Dokument.

```csharp
public TextReader GetText()
```

### Rückgabewert

Eine Instanz vonTextReader Klasse mit dem extrahierten Text; `Null` wenn die Textextraktion nicht unterstützt wird.

### Bemerkungen

**Erfahren Sie mehr:**

* [Text aus Dokumenten extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [Extrahieren Sie Text im genauen Modus](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Beispiele

Das folgende Beispiel zeigt, wie Sie einen Text aus einem Dokument extrahieren:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse
using(Parser parser = new Parser(filePath))
{
    // Einen Text in den Reader extrahieren
    using(TextReader reader = parser.GetText())
    {
        // Einen Text aus dem Dokument drucken
        // Wenn die Textextraktion nicht unterstützt wird, ist ein Reader null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Siehe auch

* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## GetText(TextOptions) {#gettext_1}

Extrahiert eine Textseite aus dem Dokument mithilfe von Textoptionen (um den Rohtext-Schnellextraktionsmodus zu aktivieren).

```csharp
public TextReader GetText(TextOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | TextOptions | Die Textextraktionsoptionen. |

### Rückgabewert

Eine Instanz vonTextReader Klasse mit dem extrahierten Text; `Null` wenn die Textextraktion nicht unterstützt wird.

### Bemerkungen

**Erfahren Sie mehr:**

* [Extrahieren Sie Text im genauen Modus](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Text im Raw-Modus extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Beispiele

Das folgende Beispiel zeigt, wie Sie einen Rohtext aus einem Dokument extrahieren:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse
using(Parser parser = new Parser(filePath))
{
    // Einen Rohtext in den Reader extrahieren
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // Einen Text aus dem Dokument drucken
        // Wenn die Textextraktion nicht unterstützt wird, ist ein Reader null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Siehe auch

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

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

Eine Instanz vonTextReader Klasse mit dem extrahierten Text; `Null` wenn die Extraktion von Textseiten nicht unterstützt wird.

### Bemerkungen

**Erfahren Sie mehr:**

* [Extrahieren Sie Text im genauen Modus](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Beispiele

Das folgende Beispiel zeigt, wie Sie einen Text aus der Dokumentseite extrahieren:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse
using(Parser parser = new Parser(filePath))
{
    // Prüfen, ob das Dokument Textextraktion unterstützt
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
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
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // Eine Seitenzahl drucken 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // Einen Text in den Reader extrahieren
        using(TextReader reader = parser.GetText(p))
        {
            // Einen Text aus dem Dokument drucken
            // Wir ignorieren die Nullprüfung, da wir zuvor die Unterstützung der Textextraktionsfunktion überprüft haben
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Siehe auch

* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## GetText(int, TextOptions) {#gettext_3}

Extrahiert einen Text aus der Dokumentseite mithilfe von Textoptionen (um den Rohtext-Schnellextraktionsmodus zu aktivieren).

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | Int32 | Der nullbasierte Seitenindex. |
| options | TextOptions | Die Textextraktionsoptionen. |

### Rückgabewert

Eine Instanz vonTextReader Klasse mit dem extrahierten Text; `Null` wenn die Extraktion von Textseiten nicht unterstützt wird.

### Bemerkungen

**Erfahren Sie mehr:**

* [Extrahieren Sie Text im genauen Modus](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Text im Raw-Modus extrahieren](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Beispiele

Das folgende Beispiel zeigt, wie Sie einen Rohtext aus der Dokumentseite extrahieren:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse
using(Parser parser = new Parser(filePath))
{
    // Prüfen, ob das Dokument Textextraktion unterstützt
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Holen Sie sich die Dokumentinformationen
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // Prüfe, ob das Dokument Seiten hat
    if(documentInfo == null || documentInfo.RawPageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Über Seiten iterieren
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // Eine Seitenzahl drucken 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // Einen Text in den Reader extrahieren
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // Einen Text aus dem Dokument drucken
            // Wir ignorieren die Nullprüfung, da wir zuvor die Unterstützung der Textextraktionsfunktion überprüft haben
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Siehe auch

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

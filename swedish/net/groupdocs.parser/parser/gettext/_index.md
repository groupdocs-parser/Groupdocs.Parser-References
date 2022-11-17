---
title: GetText
second_title: GroupDocs.Parser för .NET API-referens
description: Extraherar en text från dokumentet.
type: docs
weight: 150
url: /sv/net/groupdocs.parser/parser/gettext/
---
## GetText() {#gettext}

Extraherar en text från dokumentet.

```csharp
public TextReader GetText()
```

### Returvärde

En instans avTextReader klass med den extraherade texten; `null` om textextraktion inte stöds.

### Anmärkningar

**Läs mer:**

* [Extrahera text från dokument](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [Extrahera text i exakt läge](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Exempel

Följande exempel visar hur man extraherar en text från ett dokument:

```csharp
// Skapa en instans av Parser-klassen
using(Parser parser = new Parser(filePath))
{
    // Extrahera en text i läsaren
    using(TextReader reader = parser.GetText())
    {
        // Skriv ut en text från dokumentet
        // Om textextraktion inte stöds är en läsare null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Se även

* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## GetText(TextOptions) {#gettext_1}

Extraherar en textsida från dokumentet med hjälp av textalternativ (för att aktivera läget för rå textextrahering).

```csharp
public TextReader GetText(TextOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| options | TextOptions | Alternativen för textextraktion. |

### Returvärde

En instans avTextReader klass med den extraherade texten; `null` om textextraktion inte stöds.

### Anmärkningar

**Läs mer:**

* [Extrahera text i exakt läge](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extrahera text i råläge](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Exempel

Följande exempel visar hur man extraherar en råtext från ett dokument:

```csharp
// Skapa en instans av Parser-klassen
using(Parser parser = new Parser(filePath))
{
    // Extrahera en råtext i läsaren
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // Skriv ut en text från dokumentet
        // Om textextraktion inte stöds är en läsare null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Se även

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

Extraherar en text från dokumentsidan.

```csharp
public TextReader GetText(int pageIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | Det nollbaserade sidindexet. |

### Returvärde

En instans avTextReader klass med den extraherade texten; `null` om extrahering av textsidor inte stöds.

### Anmärkningar

**Läs mer:**

* [Extrahera text i exakt läge](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Exempel

Följande exempel visar hur man extraherar en text från dokumentsidan:

```csharp
// Skapa en instans av Parser-klassen
using(Parser parser = new Parser(filePath))
{
    // Kontrollera om dokumentet stöder textextraktion
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Få dokumentinformationen
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Kontrollera om dokumentet har sidor
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Iterera över sidor
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // Skriv ut ett sidnummer 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // Extrahera en text i läsaren
        using(TextReader reader = parser.GetText(p))
        {
            // Skriv ut en text från dokumentet
            // Vi ignorerar nollkontroll eftersom vi har kontrollerat stöd för textextrahering tidigare
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Se även

* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## GetText(int, TextOptions) {#gettext_3}

Extraherar en text från dokumentsidan med hjälp av textalternativ (för att aktivera råsnabbt textextraktionsläge).

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | Det nollbaserade sidindexet. |
| options | TextOptions | Alternativen för textextraktion. |

### Returvärde

En instans avTextReader klass med den extraherade texten; `null` om extrahering av textsidor inte stöds.

### Anmärkningar

**Läs mer:**

* [Extrahera text i exakt läge](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extrahera text i råläge](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Exempel

Följande exempel visar hur man extraherar en råtext från dokumentsidan:

```csharp
// Skapa en instans av Parser-klassen
using(Parser parser = new Parser(filePath))
{
    // Kontrollera om dokumentet stöder textextraktion
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Få dokumentinformationen
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // Kontrollera om dokumentet har sidor
    if(documentInfo == null || documentInfo.RawPageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Iterera över sidor
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // Skriv ut ett sidnummer 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // Extrahera en text i läsaren
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // Skriv ut en text från dokumentet
            // Vi ignorerar nollkontroll eftersom vi har kontrollerat stöd för textextrahering tidigare
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Se även

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

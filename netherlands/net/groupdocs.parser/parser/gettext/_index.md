---
title: GetText
second_title: GroupDocs.Parser voor .NET API-referentie
description: Extraheert een tekst uit het document.
type: docs
weight: 150
url: /nl/net/groupdocs.parser/parser/gettext/
---
## GetText() {#gettext}

Extraheert een tekst uit het document.

```csharp
public TextReader GetText()
```

### Winstwaarde

Een exemplaar vanTextReader klasse met de geëxtraheerde tekst; `nul` als tekstextractie niet wordt ondersteund.

### Opmerkingen

**Kom meer te weten:**

* [Extraheer tekst uit documenten](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [Extraheer tekst in de modus Nauwkeurig](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Voorbeelden

Het volgende voorbeeld laat zien hoe u een tekst uit een document haalt:

```csharp
// Maak een instantie van de Parser-klasse
using(Parser parser = new Parser(filePath))
{
    // Extraheer een tekst in de reader
    using(TextReader reader = parser.GetText())
    {
        // Print een tekst uit het document
        // Als tekstextractie niet wordt ondersteund, is een lezer null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Zie ook

* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## GetText(TextOptions) {#gettext_1}

Extraheert een tekstpagina uit het document met behulp van tekstopties (om de modus Raw Fast Text Extraction in te schakelen).

```csharp
public TextReader GetText(TextOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| options | TextOptions | De opties voor tekstextractie. |

### Winstwaarde

Een exemplaar vanTextReader klasse met de geëxtraheerde tekst; `nul` als tekstextractie niet wordt ondersteund.

### Opmerkingen

**Kom meer te weten:**

* [Extraheer tekst in de modus Nauwkeurig](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extraheer tekst in Raw-modus](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Voorbeelden

Het volgende voorbeeld laat zien hoe u een onbewerkte tekst uit een document haalt:

```csharp
// Maak een instantie van de Parser-klasse
using(Parser parser = new Parser(filePath))
{
    // Extraheer een onbewerkte tekst in de lezer
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // Print een tekst uit het document
        // Als tekstextractie niet wordt ondersteund, is een lezer null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Zie ook

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

Extraheert een tekst van de documentpagina.

```csharp
public TextReader GetText(int pageIndex)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageIndex | Int32 | De op nul gebaseerde pagina-index. |

### Winstwaarde

Een exemplaar vanTextReader klasse met de geëxtraheerde tekst; `nul` als tekstpagina-extractie niet wordt ondersteund.

### Opmerkingen

**Kom meer te weten:**

* [Extraheer tekst in de modus Nauwkeurig](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Voorbeelden

Het volgende voorbeeld laat zien hoe een tekst uit de documentpagina gehaald kan worden:

```csharp
// Maak een instantie van de Parser-klasse
using(Parser parser = new Parser(filePath))
{
    // Controleer of het document tekstextractie ondersteunt
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Haal de documentinfo op
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Controleer of het document pagina's heeft
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Herhaal pagina's
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // Druk een paginanummer af 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // Extraheer een tekst in de reader
        using(TextReader reader = parser.GetText(p))
        {
            // Print een tekst uit het document
            // We negeren null-check omdat we eerder de ondersteuning voor tekstextractie hebben gecontroleerd
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Zie ook

* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## GetText(int, TextOptions) {#gettext_3}

Extraheert een tekst van de documentpagina met behulp van tekstopties (om de modus Raw Fast Text Extraction in te schakelen).

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageIndex | Int32 | De op nul gebaseerde pagina-index. |
| options | TextOptions | De opties voor tekstextractie. |

### Winstwaarde

Een exemplaar vanTextReader klasse met de geëxtraheerde tekst; `nul` als tekstpagina-extractie niet wordt ondersteund.

### Opmerkingen

**Kom meer te weten:**

* [Extraheer tekst in de modus Nauwkeurig](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extraheer tekst in Raw-modus](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Voorbeelden

Het volgende voorbeeld laat zien hoe u een onbewerkte tekst uit de documentpagina haalt:

```csharp
// Maak een instantie van de Parser-klasse
using(Parser parser = new Parser(filePath))
{
    // Controleer of het document tekstextractie ondersteunt
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Haal de documentinfo op
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // Controleer of het document pagina's heeft
    if(documentInfo == null || documentInfo.RawPageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Herhaal pagina's
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // Druk een paginanummer af 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // Extraheer een tekst in de reader
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // Print een tekst uit het document
            // We negeren null-check omdat we eerder de ondersteuning voor tekstextractie hebben gecontroleerd
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Zie ook

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

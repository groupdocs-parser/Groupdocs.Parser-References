---
title: "GetText"
second_title: "GroupDocs.Parser voor .NET API-referentie"
description: "Extraheert een tekst uit het document."
type: docs
weight: 180
url: /nl/net/groupdocs.parser/parser/gettext/
---

## GetText() {#gettext}

Extraheert een tekst uit het document.

```csharp
public TextReader GetText()
```

### Retourwaarde

Een instantie van de TextReader-klasse met de geëxtraheerde tekst; `null` als tekstextractie niet wordt ondersteund.

### Opmerkingen

**Learn more:**

* [Extract text from documents](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Voorbeelden

Het volgende voorbeeld toont hoe een tekst uit een document te extraheren:

```csharp
// Maak een instantie van de Parser‑klasse
using(Parser parser = new Parser(filePath))
{
    // Extraheer een tekst naar de reader
    using(TextReader reader = parser.GetText())
    {
        // Print een tekst uit het document
        // Als tekstextractie niet wordt ondersteund, is een reader `null`
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Zie ook

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(TextOptions) {#gettext_1}

Extraheert een tekspagina uit het document met behulp van tekstopties (om de ruwe snelle tekstelextractiemodus in te schakelen).

```csharp
public TextReader GetText(TextOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| options | TextOptions | De tekstextractie-opties. |

### Retourwaarde

Een instantie van de TextReader-klasse met de geëxtraheerde tekst; `null` als tekstextractie niet wordt ondersteund.

### Opmerkingen

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Voorbeelden

Het volgende voorbeeld toont hoe een ruwe tekst uit een document te extraheren:

```csharp
// Maak een instantie van de Parser‑klasse
using(Parser parser = new Parser(filePath))
{
    // Extraheer een ruwe tekst naar de reader
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // Print een tekst uit het document
        // Als tekstextractie niet wordt ondersteund, is een reader `null`
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Zie ook

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

Extraheert een tekst van de documentpagina.

```csharp
public TextReader GetText(int pageIndex)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageIndex | Int32 | De nulgebaseerde paginapositie. |

### Retourwaarde

Een instantie van de TextReader-klasse met de geëxtraheerde tekst; `null` als paginatekstextractie niet wordt ondersteund.

### Opmerkingen

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Voorbeelden

Het volgende voorbeeld toont hoe een tekst uit de documentpagina te extraheren:

```csharp
// Maak een instantie van de Parser‑klasse
using(Parser parser = new Parser(filePath))
{
    // Controleer of het document tekstextractie ondersteunt
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Haal de documentinformatie op
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Controleer of het document pagina's heeft
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Itereer over pagina's
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // Print een paginanummer 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // Extraheer een tekst naar de reader
        using(TextReader reader = parser.GetText(p))
        {
            // Print een tekst uit het document
            // We negeren null-controle omdat we eerder de ondersteuning voor tekstextractie hebben gecontroleerd
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Zie ook

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(int, TextOptions) {#gettext_3}

Extraheert een tekst van de documentpagina met behulp van tekstopties (om de ruwe snelle tekstelextractiemodus in te schakelen).

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageIndex | Int32 | De nulgebaseerde paginapositie. |
| options | TextOptions | De tekstextractie-opties. |

### Retourwaarde

Een instantie van de TextReader-klasse met de geëxtraheerde tekst; `null` als paginatekstextractie niet wordt ondersteund.

### Opmerkingen

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Voorbeelden

Het volgende voorbeeld toont hoe een ruwe tekst uit de documentpagina te extraheren:

```csharp
// Maak een instantie van de Parser‑klasse
using(Parser parser = new Parser(filePath))
{
    // Controleer of het document tekstextractie ondersteunt
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Haal de documentinformatie op
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // Controleer of het document pagina's heeft
    if(documentInfo == null || documentInfo.RawPageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Itereer over pagina's
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // Print een paginanummer 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // Extraheer een tekst naar de reader
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // Print een tekst uit het document
            // We negeren null-controle omdat we eerder de ondersteuning voor tekstextractie hebben gecontroleerd
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Zie ook

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

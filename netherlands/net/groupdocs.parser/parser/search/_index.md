---
title: Search
second_title: GroupDocs.Parser voor .NET API-referentie
description: Zoekt eenkeyword in het document.
type: docs
weight: 200
url: /nl/net/groupdocs.parser/parser/search/
---
## Search(string) {#search}

Zoekt een*keyword* in het document.

```csharp
public IEnumerable<SearchResult> Search(string keyword)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| keyword | String | Het trefwoord om te zoeken. |

### Winstwaarde

Een verzameling van[`SearchResult`](../../../groupdocs.parser.data/searchresult) voorwerpen; `nul` als zoeken niet wordt ondersteund.

### Opmerkingen

**Kom meer te weten:**

* [Zoek tekst](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Zoek tekst in Microsoft Office Word-documenten](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Zoek tekst in Microsoft Office Excel-spreadsheets](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Zoek tekst in Microsoft Office PowerPoint-presentaties](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Zoek tekst in PDF-documenten](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Zoek tekst in e-mails](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Zoek tekst in EPUB eBooks](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Zoek tekst in HTML-documenten](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Zoek tekst in Microsoft OneNote-secties](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Voorbeelden

Het volgende voorbeeld laat zien hoe u een trefwoord in een document kunt vinden:

```csharp
// Maak een instantie van de Parser-klasse
using(Parser parser = new Parser(filePath))
{
    // Zoek een trefwoord:
    IEnumerable<SearchResult> sr = parser.Search("page number");
    // Controleer of zoeken wordt ondersteund
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Herhaal de zoekresultaten
    foreach(SearchResult s in sr)
    {
        // Druk een index en gevonden tekst af:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

### Zie ook

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## Search(string, SearchOptions) {#search_1}

Zoekt een*keyword*in het document met behulp van zoekopties (reguliere expressie, hoofdlettergebruik, etc.).

```csharp
public IEnumerable<SearchResult> Search(string keyword, SearchOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| keyword | String | Het trefwoord om te zoeken. |
| options | SearchOptions | De zoekmogelijkheden. |

### Winstwaarde

Een verzameling van[`SearchResult`](../../../groupdocs.parser.data/searchresult) objecten; `nul` als zoeken niet wordt ondersteund.

### Opmerkingen

**Kom meer te weten:**

* [Zoek tekst](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Zoek tekst in Microsoft Office Word-documenten](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Zoek tekst in Microsoft Office Excel-spreadsheets](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Zoek tekst in Microsoft Office PowerPoint-presentaties](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Zoek tekst in PDF-documenten](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Zoek tekst in e-mails](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Zoek tekst in EPUB eBooks](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Zoek tekst in HTML-documenten](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Zoek tekst in Microsoft OneNote-secties](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Voorbeelden

Het volgende voorbeeld laat zien hoe u kunt zoeken met een reguliere expressie in een document:

In het volgende voorbeeld ziet u hoe u een tekst op pagina's kunt doorzoeken:

```csharp
// Maak een instantie van de Parser-klasse
using(Parser parser = new Parser(filePath))
{
    // Zoeken met een reguliere expressie met hoofdlettergebruik
    IEnumerable<SearchResult> sr = parser.Search("page number: [0-9]+", new SearchOptions(true, false, true));
    // Controleer of zoeken wordt ondersteund
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Herhaal de zoekresultaten
    foreach(SearchResult s in sr)
    {
        // Druk een index en gevonden tekst af:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

```csharp
// Maak een instantie van de Parser-klasse
using(Parser parser = new Parser(filePath))
{
    // Zoek een trefwoord met paginanummers
    IEnumerable<SearchResult> sr = parser.Search("line", new SearchOptions(false, false, false, true));
    // Controleer of zoeken wordt ondersteund
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Herhaal de zoekresultaten
    foreach(SearchResult s in sr)
    {
        // Druk een index, paginanummer en gevonden tekst af:
        Console.WriteLine(string.Format("At {0} (page {1}): {2}", s.Position, s.PageIndex, s.Text));
    }
}
```

### Zie ook

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [SearchOptions](../../../groupdocs.parser.options/searchoptions)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

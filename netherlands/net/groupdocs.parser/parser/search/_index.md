---
title: "Search"
second_title: "GroupDocs.Parser voor .NET API-referentie"
description: "Zoekt een trefwoord in het document."
type: docs
weight: 250
url: /nl/net/groupdocs.parser/parser/search/
---

## Search(string) {#search}

Zoekt een *keyword* in het document.

```csharp
public IEnumerable<SearchResult> Search(string keyword)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| trefwoord | String | Het trefwoord om te zoeken. |

### Retourwaarde

Een collectie van [`SearchResult`](../../../groupdocs.parser.data/searchresult) objecten; `null` als zoeken niet wordt ondersteund.

### Opmerkingen

**Learn more:**

* [Search text](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Search text in Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Search text in Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Search text in Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Search text in PDF documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Search text in Emails](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Search text in EPUB eBooks](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Search text in HTML documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Search text in Microsoft OneNote sections](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Voorbeelden

Het volgende voorbeeld toont hoe een trefwoord in een document te vinden is:

```csharp
// Maak een instantie van de Parser‑klasse
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
 
    // Itereer over zoekresultaten
    foreach(SearchResult s in sr)
    {
        // Print een index en gevonden tekst:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

### Zie ook

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Search(string, SearchOptions) {#search_1}

Zoekt een *keyword* in het document met behulp van zoekopties (reguliere expressie, hoofdlettergevoeligheid, enz.).

```csharp
public IEnumerable<SearchResult> Search(string keyword, SearchOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| trefwoord | String | Het trefwoord om te zoeken. |
| options | SearchOptions | De zoekopties. |

### Retourwaarde

Een collectie van [`SearchResult`](../../../groupdocs.parser.data/searchresult) objecten; `null` als zoeken niet wordt ondersteund.

### Opmerkingen

**Learn more:**

* [Search text](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Search text in Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Search text in Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Search text in Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Search text in PDF documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Search text in Emails](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Search text in EPUB eBooks](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Search text in HTML documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Search text in Microsoft OneNote sections](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Voorbeelden

Het volgende voorbeeld toont hoe te zoeken met een reguliere expressie in een document:

```csharp
// Maak een instantie van de Parser‑klasse
using(Parser parser = new Parser(filePath))
{
    // Zoeken met een reguliere expressie met hoofdlettergevoeligheid
    IEnumerable<SearchResult> sr = parser.Search("page number: [0-9]+", new SearchOptions(true, false, true));
    // Controleer of zoeken wordt ondersteund
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Itereer over zoekresultaten
    foreach(SearchResult s in sr)
    {
        // Print een index en gevonden tekst:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

Het volgende voorbeeld toont hoe tekst te zoeken op pagina's:

```csharp
// Maak een instantie van de Parser‑klasse
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
 
    // Itereer over zoekresultaten
    foreach(SearchResult s in sr)
    {
        // Print een index, paginanummer en gevonden tekst:
        Console.WriteLine(string.Format("At {0} (page {1}): {2}", s.Position, s.PageIndex, s.Text));
    }
}
```

### Zie ook

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [SearchOptions](../../../groupdocs.parser.options/searchoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

---
title: Search
second_title: GroupDocs.Parser för .NET API-referens
description: Söker akeyword i dokumentet.
type: docs
weight: 200
url: /sv/net/groupdocs.parser/parser/search/
---
## Search(string) {#search}

Söker a*keyword* i dokumentet.

```csharp
public IEnumerable<SearchResult> Search(string keyword)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| keyword | String | Nyckelordet att söka. |

### Returvärde

En samling av[`SearchResult`](../../../groupdocs.parser.data/searchresult) föremål; `null` om sökning inte stöds.

### Anmärkningar

**Läs mer:**

* [Sök text](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Sök text i Microsoft Office Word-dokument](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Sök text i Microsoft Office Excel-kalkylblad](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Sök text i Microsoft Office PowerPoint-presentationer](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Sök text i PDF-dokument](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Sök text i e-postmeddelanden](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Sök text i EPUB e-böcker](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Sök text i HTML-dokument](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Sök text i Microsoft OneNote-sektioner](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Exempel

Följande exempel visar hur du hittar ett nyckelord i ett dokument:

```csharp
// Skapa en instans av Parser-klassen
using(Parser parser = new Parser(filePath))
{
    // Sök efter ett nyckelord:
    IEnumerable<SearchResult> sr = parser.Search("page number");
    // Kontrollera om sökning stöds
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Iterera över sökresultat
    foreach(SearchResult s in sr)
    {
        // Skriv ut ett index och hittad text:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

### Se även

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## Search(string, SearchOptions) {#search_1}

Söker a*keyword* dokumentet med hjälp av sökalternativ (reguljärt uttryck, matcha skiftläge, etc.).

```csharp
public IEnumerable<SearchResult> Search(string keyword, SearchOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| keyword | String | Nyckelordet att söka. |
| options | SearchOptions | Sökalternativen. |

### Returvärde

En samling av[`SearchResult`](../../../groupdocs.parser.data/searchresult) objekt; `null` om sökning inte stöds.

### Anmärkningar

**Läs mer:**

* [Sök text](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Sök text i Microsoft Office Word-dokument](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Sök text i Microsoft Office Excel-kalkylblad](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Sök text i Microsoft Office PowerPoint-presentationer](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Sök text i PDF-dokument](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Sök text i e-postmeddelanden](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Sök text i EPUB e-böcker](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Sök text i HTML-dokument](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Sök text i Microsoft OneNote-sektioner](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Exempel

Följande exempel visar hur man söker med ett reguljärt uttryck i ett dokument:

Följande exempel visar hur man söker efter en text på sidor:

```csharp
// Skapa en instans av Parser-klassen
using(Parser parser = new Parser(filePath))
{
    // Sök med ett reguljärt uttryck med skiftlägesmatchning
    IEnumerable<SearchResult> sr = parser.Search("page number: [0-9]+", new SearchOptions(true, false, true));
    // Kontrollera om sökning stöds
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Iterera över sökresultat
    foreach(SearchResult s in sr)
    {
        // Skriv ut ett index och hittad text:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

```csharp
// Skapa en instans av Parser-klassen
using(Parser parser = new Parser(filePath))
{
    // Sök efter ett nyckelord med sidnummer
    IEnumerable<SearchResult> sr = parser.Search("line", new SearchOptions(false, false, false, true));
    // Kontrollera om sökning stöds
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Iterera över sökresultat
    foreach(SearchResult s in sr)
    {
        // Skriv ut ett index, sidnummer och hittad text:
        Console.WriteLine(string.Format("At {0} (page {1}): {2}", s.Position, s.PageIndex, s.Text));
    }
}
```

### Se även

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [SearchOptions](../../../groupdocs.parser.options/searchoptions)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

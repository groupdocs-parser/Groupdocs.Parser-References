---
title: Search
second_title: GroupDocs.Parser für .NET-API-Referenz
description: Sucht akeyword im Dokument.
type: docs
weight: 200
url: /de/net/groupdocs.parser/parser/search/
---
## Search(string) {#search}

Sucht a*keyword* im Dokument.

```csharp
public IEnumerable<SearchResult> Search(string keyword)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| keyword | String | Das zu suchende Schlüsselwort. |

### Rückgabewert

Eine Sammlung von[`SearchResult`](../../../groupdocs.parser.data/searchresult) Gegenstände; `Null` wenn die Suche nicht unterstützt wird.

### Bemerkungen

**Erfahren Sie mehr:**

* [Suchtext](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Durchsuchen Sie Text in Microsoft Office Word-Dokumenten](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Durchsuchen Sie Text in Microsoft Office Excel-Tabellen](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Durchsuchen Sie Text in Microsoft Office PowerPoint-Präsentationen](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Text in PDF-Dokumenten suchen](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Text in E-Mails suchen](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Suchen Sie Text in EPUB-eBooks](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Text in HTML-Dokumenten suchen](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Suchen Sie Text in Microsoft OneNote-Abschnitten](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Beispiele

Das folgende Beispiel zeigt, wie Sie ein Schlüsselwort in einem Dokument finden:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse
using(Parser parser = new Parser(filePath))
{
    // Suche nach einem Schlüsselwort:
    IEnumerable<SearchResult> sr = parser.Search("page number");
    // Prüfen, ob die Suche unterstützt wird
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Suchergebnisse durchlaufen
    foreach(SearchResult s in sr)
    {
        // Index und gefundenen Text drucken:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

### Siehe auch

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## Search(string, SearchOptions) {#search_1}

Sucht a*keyword*im Dokument über Suchoptionen (regulärer Ausdruck, Groß-/Kleinschreibung etc.).

```csharp
public IEnumerable<SearchResult> Search(string keyword, SearchOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| keyword | String | Das zu suchende Schlüsselwort. |
| options | SearchOptions | Die Suchoptionen. |

### Rückgabewert

Eine Sammlung von[`SearchResult`](../../../groupdocs.parser.data/searchresult) Objekte; `Null` wenn die Suche nicht unterstützt wird.

### Bemerkungen

**Erfahren Sie mehr:**

* [Suchtext](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Durchsuchen Sie Text in Microsoft Office Word-Dokumenten](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Durchsuchen Sie Text in Microsoft Office Excel-Tabellen](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Durchsuchen Sie Text in Microsoft Office PowerPoint-Präsentationen](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Text in PDF-Dokumenten suchen](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Text in E-Mails suchen](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Suchen Sie Text in EPUB-eBooks](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Text in HTML-Dokumenten suchen](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Suchen Sie Text in Microsoft OneNote-Abschnitten](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Beispiele

Das folgende Beispiel zeigt, wie Sie mit einem regulären Ausdruck in einem Dokument suchen:

Das folgende Beispiel zeigt, wie Sie einen Text auf Seiten suchen:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse
using(Parser parser = new Parser(filePath))
{
    // Suche mit einem regulären Ausdruck mit Groß-/Kleinschreibung
    IEnumerable<SearchResult> sr = parser.Search("page number: [0-9]+", new SearchOptions(true, false, true));
    // Prüfen, ob die Suche unterstützt wird
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Suchergebnisse durchlaufen
    foreach(SearchResult s in sr)
    {
        // Index und gefundenen Text drucken:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse
using(Parser parser = new Parser(filePath))
{
    // Suchen Sie ein Schlüsselwort mit Seitenzahlen
    IEnumerable<SearchResult> sr = parser.Search("line", new SearchOptions(false, false, false, true));
    // Prüfen, ob die Suche unterstützt wird
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Suchergebnisse durchlaufen
    foreach(SearchResult s in sr)
    {
        // Index, Seitennummer und gefundenen Text drucken:
        Console.WriteLine(string.Format("At {0} (page {1}): {2}", s.Position, s.PageIndex, s.Text));
    }
}
```

### Siehe auch

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [SearchOptions](../../../groupdocs.parser.options/searchoptions)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

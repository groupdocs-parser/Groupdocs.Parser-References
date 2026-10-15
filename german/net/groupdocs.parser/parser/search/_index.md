---
title: "Suche"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Durchsucht ein Schlüsselwort im Dokument."
type: docs
weight: 250
url: /de/net/groupdocs.parser/parser/search/
---

## Search(string) {#search}

Durchsucht ein *keyword* im Dokument.

```csharp
public IEnumerable<SearchResult> Search(string keyword)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Schlüsselwort | String | Das zu suchende Schlüsselwort. |

### Rückgabewert

Eine Sammlung von [`SearchResult`](../../../groupdocs.parser.data/searchresult)-Objekten; `null`, wenn die Suche nicht unterstützt wird.

### Hinweise

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

### Beispiele

Das folgende Beispiel zeigt, wie man ein Schlüsselwort in einem Dokument findet:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using(Parser parser = new Parser(filePath))
{
    // Suche ein Schlüsselwort:
    IEnumerable<SearchResult> sr = parser.Search("page number");
    // Prüfe, ob die Suche unterstützt wird
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Iteriere über die Suchergebnisse
    foreach(SearchResult s in sr)
    {
        // Gib einen Index und den gefundenen Text aus:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

### Siehe auch

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Search(string, SearchOptions) {#search_1}

Durchsucht ein *keyword* im Dokument unter Verwendung von Suchoptionen (regulärer Ausdruck, Groß-/Kleinschreibung beachten usw.).

```csharp
public IEnumerable<SearchResult> Search(string keyword, SearchOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Schlüsselwort | String | Das zu suchende Schlüsselwort. |
| options | SearchOptions | Die Suchoptionen. |

### Rückgabewert

Eine Sammlung von [`SearchResult`](../../../groupdocs.parser.data/searchresult)-Objekten; `null`, wenn die Suche nicht unterstützt wird.

### Hinweise

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

### Beispiele

Das folgende Beispiel zeigt, wie man mit einem regulären Ausdruck in einem Dokument sucht:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using(Parser parser = new Parser(filePath))
{
    // Suche mit einem regulären Ausdruck unter Berücksichtigung der Groß-/Kleinschreibung
    IEnumerable<SearchResult> sr = parser.Search("page number: [0-9]+", new SearchOptions(true, false, true));
    // Prüfe, ob die Suche unterstützt wird
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Iteriere über die Suchergebnisse
    foreach(SearchResult s in sr)
    {
        // Gib einen Index und den gefundenen Text aus:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

Das folgende Beispiel zeigt, wie man einen Text auf Seiten sucht:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using(Parser parser = new Parser(filePath))
{
    // Suche ein Schlüsselwort mit Seitenzahlen
    IEnumerable<SearchResult> sr = parser.Search("line", new SearchOptions(false, false, false, true));
    // Prüfe, ob die Suche unterstützt wird
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Iteriere über die Suchergebnisse
    foreach(SearchResult s in sr)
    {
        // Gib einen Index, die Seitenzahl und den gefundenen Text aus:
        Console.WriteLine(string.Format("At {0} (page {1}): {2}", s.Position, s.PageIndex, s.Text));
    }
}
```

### Siehe auch

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [SearchOptions](../../../groupdocs.parser.options/searchoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->

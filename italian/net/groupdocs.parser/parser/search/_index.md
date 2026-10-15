---
title: "Ricerca"
second_title: "Riferimento API di GroupDocs.Parser per .NET"
description: "Cerca una parola chiave nel documento."
type: docs
weight: 250
url: /it/net/groupdocs.parser/parser/search/
---

## Search(string) {#search}

Cerca una *keyword* nel documento.

```csharp
public IEnumerable<SearchResult> Search(string keyword)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| parola chiave | Stringa | La parola chiave da cercare. |

### Valore di ritorno

Una collezione di oggetti [`SearchResult`](../../../groupdocs.parser.data/searchresult); `null` se la ricerca non è supportata.

### Osservazioni

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

### Esempi

Il seguente esempio mostra come trovare una parola chiave in un documento:

```csharp
// Crea un'istanza della classe Parser
using(Parser parser = new Parser(filePath))
{
    // Cerca una parola chiave:
    IEnumerable<SearchResult> sr = parser.Search("page number");
    // Verifica se la ricerca è supportata
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Itera sui risultati della ricerca
    foreach(SearchResult s in sr)
    {
        // Stampa un indice e il testo trovato:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

### Vedi anche

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Search(string, SearchOptions) {#search_1}

Cerca una *keyword* nel documento usando opzioni di ricerca (espressione regolare, distinzione maiuscole/minuscole, ecc.).

```csharp
public IEnumerable<SearchResult> Search(string keyword, SearchOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| parola chiave | Stringa | La parola chiave da cercare. |
| options | SearchOptions | Le opzioni di ricerca. |

### Valore di ritorno

Una collezione di oggetti [`SearchResult`](../../../groupdocs.parser.data/searchresult); `null` se la ricerca non è supportata.

### Osservazioni

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

### Esempi

Il seguente esempio mostra come cercare con un'espressione regolare in un documento:

```csharp
// Crea un'istanza della classe Parser
using(Parser parser = new Parser(filePath))
{
    // Cerca con un'espressione regolare con corrispondenza di maiuscole/minuscole
    IEnumerable<SearchResult> sr = parser.Search("page number: [0-9]+", new SearchOptions(true, false, true));
    // Verifica se la ricerca è supportata
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Itera sui risultati della ricerca
    foreach(SearchResult s in sr)
    {
        // Stampa un indice e il testo trovato:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

Il seguente esempio mostra come cercare un testo nelle pagine:

```csharp
// Crea un'istanza della classe Parser
using(Parser parser = new Parser(filePath))
{
    // Cerca una parola chiave con i numeri di pagina
    IEnumerable<SearchResult> sr = parser.Search("line", new SearchOptions(false, false, false, true));
    // Verifica se la ricerca è supportata
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Itera sui risultati della ricerca
    foreach(SearchResult s in sr)
    {
        // Stampa un indice, il numero di pagina e il testo trovato:
        Console.WriteLine(string.Format("At {0} (page {1}): {2}", s.Position, s.PageIndex, s.Text));
    }
}
```

### Vedi anche

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [SearchOptions](../../../groupdocs.parser.options/searchoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

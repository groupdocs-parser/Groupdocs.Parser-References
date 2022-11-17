---
title: Search
second_title: Riferimento API GroupDocs.Parser per .NET
description: Ricerche akeyword nel documento.
type: docs
weight: 200
url: /it/net/groupdocs.parser/parser/search/
---
## Search(string) {#search}

Ricerche a*keyword* nel documento.

```csharp
public IEnumerable<SearchResult> Search(string keyword)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| keyword | String | La parola chiave da cercare. |

### Valore di ritorno

Una raccolta di[`SearchResult`](../../../groupdocs.parser.data/searchresult) oggetti; `nullo` se la ricerca non è supportata.

### Osservazioni

**Scopri di più:**

* [Cerca testo](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Cerca testo nei documenti di Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Cerca testo nei fogli di calcolo di Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Cerca testo nelle presentazioni di Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Cerca testo nei documenti PDF](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Cerca testo nelle e-mail](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Cerca il testo negli eBook EPUB](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Cerca testo nei documenti HTML](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Cerca testo nelle sezioni di Microsoft OneNote](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Esempi

L'esempio seguente mostra come trovare una parola chiave in un documento:

```csharp
// Crea un'istanza della classe Parser
using(Parser parser = new Parser(filePath))
{
    // Cerca una parola chiave:
    IEnumerable<SearchResult> sr = parser.Search("page number");
    // Controlla se la ricerca è supportata
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

### Guarda anche

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

---

## Search(string, SearchOptions) {#search_1}

Ricerche a*keyword*nel documento utilizzando le opzioni di ricerca (espressione regolare, match case, ecc.).

```csharp
public IEnumerable<SearchResult> Search(string keyword, SearchOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| keyword | String | La parola chiave da cercare. |
| options | SearchOptions | Le opzioni di ricerca. |

### Valore di ritorno

Una raccolta di[`SearchResult`](../../../groupdocs.parser.data/searchresult) oggetti; `nullo` se la ricerca non è supportata.

### Osservazioni

**Scopri di più:**

* [Cerca testo](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Cerca testo nei documenti di Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Cerca testo nei fogli di calcolo di Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Cerca testo nelle presentazioni di Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Cerca testo nei documenti PDF](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Cerca testo nelle e-mail](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Cerca il testo negli eBook EPUB](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Cerca testo nei documenti HTML](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Cerca testo nelle sezioni di Microsoft OneNote](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Esempi

L'esempio seguente mostra come cercare con un'espressione regolare in un documento:

L'esempio seguente mostra come cercare un testo nelle pagine:

```csharp
// Crea un'istanza della classe Parser
using(Parser parser = new Parser(filePath))
{
    // Cerca con un'espressione regolare con corrispondenza tra maiuscole e minuscole
    IEnumerable<SearchResult> sr = parser.Search("page number: [0-9]+", new SearchOptions(true, false, true));
    // Controlla se la ricerca è supportata
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

```csharp
// Crea un'istanza della classe Parser
using(Parser parser = new Parser(filePath))
{
    // Cerca una parola chiave con i numeri di pagina
    IEnumerable<SearchResult> sr = parser.Search("line", new SearchOptions(false, false, false, true));
    // Controlla se la ricerca è supportata
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Itera sui risultati della ricerca
    foreach(SearchResult s in sr)
    {
        // Stampa un indice, numero di pagina e testo trovato:
        Console.WriteLine(string.Format("At {0} (page {1}): {2}", s.Position, s.PageIndex, s.Text));
    }
}
```

### Guarda anche

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [SearchOptions](../../../groupdocs.parser.options/searchoptions)
* class [Parser](../../parser)
* spazio dei nomi [GroupDocs.Parser](../../parser)
* assemblea [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

---
title: "Recherche"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Recherche un mot‑clé dans le document."
type: docs
weight: 250
url: /fr/net/groupdocs.parser/parser/search/
---

## Search(string) {#search}

Recherche un *mot‑clé* dans le document.

```csharp
public IEnumerable<SearchResult> Search(string keyword)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| mot‑clé | Chaîne | Le mot‑clé à rechercher. |

### Valeur de retour

Une collection d'objets [`SearchResult`](../../../groupdocs.parser.data/searchresult) ; `null` si la recherche n'est pas prise en charge.

### Remarques

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

### Exemples

L'exemple suivant montre comment trouver un mot‑clé dans un document :

```csharp
// Créez une instance de la classe Parser
using(Parser parser = new Parser(filePath))
{
    // Rechercher un mot‑clé :
    IEnumerable<SearchResult> sr = parser.Search("page number");
    // Vérifier si la recherche est prise en charge
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Parcourir les résultats de recherche
    foreach(SearchResult s in sr)
    {
        // Afficher un index et le texte trouvé :
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

### Voir aussi

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Search(string, SearchOptions) {#search_1}

Recherche un *mot‑clé* dans le document en utilisant des options de recherche (expression régulière, respect de la casse, etc.).

```csharp
public IEnumerable<SearchResult> Search(string keyword, SearchOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| mot‑clé | Chaîne | Le mot‑clé à rechercher. |
| options | SearchOptions | Les options de recherche. |

### Valeur de retour

Une collection d'objets [`SearchResult`](../../../groupdocs.parser.data/searchresult) ; `null` si la recherche n'est pas prise en charge.

### Remarques

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

### Exemples

L'exemple suivant montre comment rechercher avec une expression régulière dans un document :

```csharp
// Créez une instance de la classe Parser
using(Parser parser = new Parser(filePath))
{
    // Rechercher avec une expression régulière en tenant compte de la casse
    IEnumerable<SearchResult> sr = parser.Search("page number: [0-9]+", new SearchOptions(true, false, true));
    // Vérifier si la recherche est prise en charge
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Parcourir les résultats de recherche
    foreach(SearchResult s in sr)
    {
        // Afficher un index et le texte trouvé :
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

L'exemple suivant montre comment rechercher un texte sur les pages :

```csharp
// Créez une instance de la classe Parser
using(Parser parser = new Parser(filePath))
{
    // Rechercher un mot-clé avec les numéros de page
    IEnumerable<SearchResult> sr = parser.Search("line", new SearchOptions(false, false, false, true));
    // Vérifier si la recherche est prise en charge
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Parcourir les résultats de recherche
    foreach(SearchResult s in sr)
    {
        // Afficher un index, le numéro de page et le texte trouvé :
        Console.WriteLine(string.Format("At {0} (page {1}): {2}", s.Position, s.PageIndex, s.Text));
    }
}
```

### Voir aussi

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [SearchOptions](../../../groupdocs.parser.options/searchoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->

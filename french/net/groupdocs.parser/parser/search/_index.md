---
title: Search
second_title: Référence de l'API GroupDocs.Parser pour .NET
description: Recherche unkeyword dans le document.
type: docs
weight: 200
url: /fr/net/groupdocs.parser/parser/search/
---
## Search(string) {#search}

Recherche un*keyword* dans le document.

```csharp
public IEnumerable<SearchResult> Search(string keyword)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| keyword | String | Le mot-clé à rechercher. |

### Return_Value

Une collection de[`SearchResult`](../../../groupdocs.parser.data/searchresult) objets; `nul` si la recherche n'est pas prise en charge.

### Remarques

**Apprendre encore plus:**

* [Texte de recherche](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Rechercher du texte dans des documents Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Rechercher du texte dans des feuilles de calcul Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Rechercher du texte dans des présentations Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Rechercher du texte dans des documents PDF](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Rechercher du texte dans les e-mails](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Rechercher du texte dans les livres électroniques EPUB](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Rechercher du texte dans des documents HTML](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Rechercher du texte dans les sections Microsoft OneNote](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Exemples

L'exemple suivant montre comment rechercher un mot-clé dans un document :

```csharp
// Crée une instance de la classe Parser
using(Parser parser = new Parser(filePath))
{
    // Rechercher un mot-clé :
    IEnumerable<SearchResult> sr = parser.Search("page number");
    // Vérifie si la recherche est prise en charge
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Itérer sur les résultats de la recherche
    foreach(SearchResult s in sr)
    {
        // Affiche un index et un texte trouvé :
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

### Voir également

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

---

## Search(string, SearchOptions) {#search_1}

Recherche un*keyword*dans le document à l'aide des options de recherche (expression régulière, correspondance de casse, etc.).

```csharp
public IEnumerable<SearchResult> Search(string keyword, SearchOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| keyword | String | Le mot-clé à rechercher. |
| options | SearchOptions | Les possibilités de recherche. |

### Return_Value

Une collection de[`SearchResult`](../../../groupdocs.parser.data/searchresult) objets ; `nul` si la recherche n'est pas prise en charge.

### Remarques

**Apprendre encore plus:**

* [Texte de recherche](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Rechercher du texte dans des documents Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Rechercher du texte dans des feuilles de calcul Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Rechercher du texte dans des présentations Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Rechercher du texte dans des documents PDF](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Rechercher du texte dans les e-mails](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Rechercher du texte dans les livres électroniques EPUB](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Rechercher du texte dans des documents HTML](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Rechercher du texte dans les sections Microsoft OneNote](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Exemples

L'exemple suivant montre comment effectuer une recherche avec une expression régulière dans un document :

L'exemple suivant montre comment rechercher un texte sur des pages :

```csharp
// Crée une instance de la classe Parser
using(Parser parser = new Parser(filePath))
{
    // Recherche avec une expression régulière avec correspondance de casse
    IEnumerable<SearchResult> sr = parser.Search("page number: [0-9]+", new SearchOptions(true, false, true));
    // Vérifie si la recherche est prise en charge
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Itérer sur les résultats de la recherche
    foreach(SearchResult s in sr)
    {
        // Affiche un index et un texte trouvé :
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

```csharp
// Crée une instance de la classe Parser
using(Parser parser = new Parser(filePath))
{
    // Recherche un mot-clé avec des numéros de page
    IEnumerable<SearchResult> sr = parser.Search("line", new SearchOptions(false, false, false, true));
    // Vérifie si la recherche est prise en charge
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Itérer sur les résultats de la recherche
    foreach(SearchResult s in sr)
    {
        // Affiche un index, un numéro de page et un texte trouvé :
        Console.WriteLine(string.Format("At {0} (page {1}): {2}", s.Position, s.PageIndex, s.Text));
    }
}
```

### Voir également

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [SearchOptions](../../../groupdocs.parser.options/searchoptions)
* class [Parser](../../parser)
* espace de noms [GroupDocs.Parser](../../parser)
* Assemblée [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

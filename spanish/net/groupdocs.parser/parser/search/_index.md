---
title: Search
second_title: Referencia de API de GroupDocs.Parser para .NET
description: Busca unkeyword en el documento.
type: docs
weight: 200
url: /es/net/groupdocs.parser/parser/search/
---
## Search(string) {#search}

Busca un*keyword* en el documento.

```csharp
public IEnumerable<SearchResult> Search(string keyword)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| keyword | String | La palabra clave a buscar. |

### Valor_devuelto

Una colección de[`SearchResult`](../../../groupdocs.parser.data/searchresult) objetos; `nulo` si la búsqueda no es compatible.

### Observaciones

**Aprende más:**

* [Buscar texto](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Buscar texto en documentos de Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Buscar texto en hojas de cálculo de Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Buscar texto en presentaciones de Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Buscar texto en documentos PDF](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Buscar texto en correos electrónicos](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Buscar texto en libros electrónicos EPUB](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Buscar texto en documentos HTML](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Buscar texto en las secciones de Microsoft OneNote](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Ejemplos

El siguiente ejemplo muestra cómo encontrar una palabra clave en un documento:

```csharp
// Crea una instancia de la clase Parser
using(Parser parser = new Parser(filePath))
{
    // Buscar una palabra clave:
    IEnumerable<SearchResult> sr = parser.Search("page number");
    // Comprobar si se admite la búsqueda
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Iterar sobre los resultados de búsqueda
    foreach(SearchResult s in sr)
    {
        // Imprime un índice y texto encontrado:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

### Ver también

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## Search(string, SearchOptions) {#search_1}

Busca un*keyword*en el documento usando las opciones de búsqueda (expresión regular, mayúsculas y minúsculas, etc.).

```csharp
public IEnumerable<SearchResult> Search(string keyword, SearchOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| keyword | String | La palabra clave a buscar. |
| options | SearchOptions | Las opciones de búsqueda. |

### Valor_devuelto

Una colección de[`SearchResult`](../../../groupdocs.parser.data/searchresult) objetos; `nulo` si la búsqueda no es compatible.

### Observaciones

**Aprende más:**

* [Buscar texto](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Buscar texto en documentos de Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Buscar texto en hojas de cálculo de Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Buscar texto en presentaciones de Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Buscar texto en documentos PDF](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Buscar texto en correos electrónicos](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Buscar texto en libros electrónicos EPUB](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Buscar texto en documentos HTML](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Buscar texto en las secciones de Microsoft OneNote](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Ejemplos

El siguiente ejemplo muestra cómo buscar con una expresión regular en un documento:

El siguiente ejemplo muestra cómo buscar un texto en las páginas:

```csharp
// Crea una instancia de la clase Parser
using(Parser parser = new Parser(filePath))
{
    // Buscar con una expresión regular con coincidencia de mayúsculas y minúsculas
    IEnumerable<SearchResult> sr = parser.Search("page number: [0-9]+", new SearchOptions(true, false, true));
    // Comprobar si se admite la búsqueda
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Iterar sobre los resultados de búsqueda
    foreach(SearchResult s in sr)
    {
        // Imprime un índice y texto encontrado:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

```csharp
// Crea una instancia de la clase Parser
using(Parser parser = new Parser(filePath))
{
    // Buscar una palabra clave con números de página
    IEnumerable<SearchResult> sr = parser.Search("line", new SearchOptions(false, false, false, true));
    // Comprobar si se admite la búsqueda
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Iterar sobre los resultados de búsqueda
    foreach(SearchResult s in sr)
    {
        // Imprime un índice, número de página y texto encontrado:
        Console.WriteLine(string.Format("At {0} (page {1}): {2}", s.Position, s.PageIndex, s.Text));
    }
}
```

### Ver también

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [SearchOptions](../../../groupdocs.parser.options/searchoptions)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

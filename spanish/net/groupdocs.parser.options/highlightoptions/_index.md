---
title: HighlightOptions
second_title: Referencia de API de GroupDocs.Parser para .NET
description: Proporciona las opciones que se utilizan para extraer un resaltado un bloque de texto alrededor del texto encontrado en escenarios de búsqueda.
type: docs
weight: 420
url: /es/net/groupdocs.parser.options/highlightoptions/
---
## HighlightOptions class

Proporciona las opciones que se utilizan para extraer un resaltado (un bloque de texto alrededor del texto encontrado en escenarios de búsqueda).

```csharp
public sealed class HighlightOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [HighlightOptions](highlightoptions#constructor)(int) | Inicializa una nueva instancia del[`HighlightOptions`](../highlightoptions) clase que se utiliza para extraer un resaltado de longitud fija. |
| [HighlightOptions](highlightoptions#constructor_1)(int?, bool) | Inicializa una nueva instancia del[`HighlightOptions`](../highlightoptions) clase que se utiliza para extraer un resaltado de línea limitada. |
| [HighlightOptions](highlightoptions#constructor_2)(int?, int) | Inicializa una nueva instancia del[`HighlightOptions`](../highlightoptions) clase que se utiliza para extraer un resaltado con el recuento de palabras fijo. |
| [HighlightOptions](highlightoptions#constructor_3)(int?, int?, bool) | Inicializa una nueva instancia del[`HighlightOptions`](../highlightoptions) clase. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [IsLineLimited](../../groupdocs.parser.options/highlightoptions/islinelimited) { get; } | Obtiene el valor que indica si la extracción de resaltado está limitada por el inicio (o el final) de una línea de texto. |
| [MaxLength](../../groupdocs.parser.options/highlightoptions/maxlength) { get; } | Obtiene una longitud máxima de texto. |
| [WordCount](../../groupdocs.parser.options/highlightoptions/wordcount) { get; } | Obtiene un número máximo de palabras. |

### Observaciones

Una instancia de[`HighlightOptions`](../highlightoptions) class se utiliza como parámetro en[`GetHighlight`](../../groupdocs.parser/parser/gethighlight) method. Vea los ejemplos de uso allí.

**Aprende más:**

* [Extraer puntos destacados](https://docs.groupdocs.com/display/parsernet/Extract+highlights)

### Ver también

* espacio de nombres [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* asamblea [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

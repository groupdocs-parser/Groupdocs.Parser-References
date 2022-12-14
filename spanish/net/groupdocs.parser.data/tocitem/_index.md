---
title: TocItem
second_title: Referencia de API de GroupDocs.Parser para .NET
description: Representa el elemento que se utiliza en la funcionalidad de extracción de la tabla de contenido.
type: docs
weight: 200
url: /es/net/groupdocs.parser.data/tocitem/
---
## TocItem class

Representa el elemento que se utiliza en la funcionalidad de extracción de la tabla de contenido.

```csharp
public class TocItem
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [TocItem](tocitem)(int, string, int?) | Inicializa una nueva instancia del[`TocItem`](../tocitem) clase. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Depth](../../groupdocs.parser.data/tocitem/depth) { get; } | Obtiene el nivel de profundidad. |
| [PageIndex](../../groupdocs.parser.data/tocitem/pageindex) { get; } | Obtiene el índice de la página. |
| [Text](../../groupdocs.parser.data/tocitem/text) { get; } | Obtiene el texto. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| virtual [ExtractText](../../groupdocs.parser.data/tocitem/extracttext)() | Extrae un texto del documento al que[`TocItem`](../tocitem) objeto se refiere. |

### Observaciones

Una instancia de[`TocItem`](../tocitem) la clase se utiliza como valor de retorno de[`GetToc`](../../groupdocs.parser/parser/gettoc) métodos. Vea los ejemplos de uso allí.

### Ver también

* espacio de nombres [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* asamblea [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

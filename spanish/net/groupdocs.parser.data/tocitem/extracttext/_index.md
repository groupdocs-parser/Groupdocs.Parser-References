---
title: ExtractText
second_title: Referencia de API de GroupDocs.Parser para .NET
description: Extrae un texto del documento al queTocItemgroupdocs.parser.data/tocitem objeto se refiere.
type: docs
weight: 50
url: /es/net/groupdocs.parser.data/tocitem/extracttext/
---
## TocItem.ExtractText method

Extrae un texto del documento al que[`TocItem`](../../tocitem) objeto se refiere.

```csharp
public virtual TextReader ExtractText()
```

### Valor_devuelto

una instancia deTextReader class con el texto extraído.

### Ejemplos

El siguiente ejemplo de cómo extraer un texto por un elemento de la tabla de contenido:

```csharp
// Crea una instancia de la clase Parser
using (Parser parser = new Parser(Constants.SampleDocxWithToc))
{
    // Obtener tabla de contenidos
    IEnumerable<TocItem> tocItems = parser.GetToc();
    // Comprobar si se admite la extracción de toc
    if (tocItems == null)
    {
        Console.WriteLine("Table of contents extraction isn't supported");
    }
    // iterar sobre elementos
    foreach (TocItem tocItem in tocItems)
    {
        // Imprime el texto del capítulo
        using (TextReader reader = tocItem.ExtractText())
        {
            Console.WriteLine("----");
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Ver también

* class [TocItem](../../tocitem)
* espacio de nombres [GroupDocs.Parser.Data](../../tocitem)
* asamblea [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

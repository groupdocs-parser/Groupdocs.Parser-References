---
title: GetMetadata
second_title: Referencia de API de GroupDocs.Parser para .NET
description: Extrae metadatos del documento.
type: docs
weight: 120
url: /es/net/groupdocs.parser/parser/getmetadata/
---
## Parser.GetMetadata method

Extrae metadatos del documento.

```csharp
public IEnumerable<MetadataItem> GetMetadata()
```

### Valor_devuelto

Una colección de elementos de metadatos; `nulo` si la extracción de metadatos no es compatible.

### Observaciones

**Aprende más:**

* [Extraer metadatos de documentos](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+documents)
* [Extraiga metadatos de documentos de Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+Word+documents)
* [Extraer metadatos de hojas de cálculo de Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+Excel+spreadsheets)
* [Extraiga metadatos de presentaciones de Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+PowerPoint+presentations)
* [Extraer metadatos de documentos PDF](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+PDF+documents)
* [Extraer metadatos de correos electrónicos](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Emails)

### Ejemplos

El siguiente ejemplo muestra cómo extraer metadatos de un documento:

```csharp
// Crea una instancia de la clase Parser
using(Parser parser = new Parser(filePath))
{
    // Extraer metadatos del documento
    IEnumerable<MetadataItem> metadata = parser.GetMetadata();
    // Comprobar si se admite la extracción de metadatos
    if(metadata == null)
    {
        Console.WriteLine("Metatada extraction isn't supported");
    }
 
    // Iterar sobre elementos de metadatos
    foreach(MetadataItem item in metadata)
    {
        // Imprime el nombre y el valor de un elemento
        Console.WriteLine(string.Format("{0}: {1}", item.Name, item.Value));
    }
}
```

### Ver también

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
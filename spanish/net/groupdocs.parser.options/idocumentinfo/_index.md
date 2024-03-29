---
title: IDocumentInfo
second_title: Referencia de API de GroupDocs.Parser para .NET
description: Representa la información del documento.
type: docs
weight: 430
url: /es/net/groupdocs.parser.options/idocumentinfo/
---
## IDocumentInfo interface

Representa la información del documento.

```csharp
public interface IDocumentInfo
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [FileType](../../groupdocs.parser.options/idocumentinfo/filetype) { get; } | Obtiene el tipo de documento. |
| [PageCount](../../groupdocs.parser.options/idocumentinfo/pagecount) { get; } | Obtiene el número total de páginas del documento. |
| [Pages](../../groupdocs.parser.options/idocumentinfo/pages) { get; } | Obtiene información sobre las páginas, como el índice y el tamaño de la página. |
| [RawPageCount](../../groupdocs.parser.options/idocumentinfo/rawpagecount) { get; } | Obtiene el número total de páginas sin procesar del documento. |
| [Size](../../groupdocs.parser.options/idocumentinfo/size) { get; } | Obtiene el tamaño del documento en bytes. |

### Observaciones

Los objetos que implementan esta interfaz son devueltos por[`GetDocumentInfo`](../../groupdocs.parser/parser/getdocumentinfo) method. Vea los ejemplos de uso allí. **Aprende más:**

* [Obtener información del documento](https://docs.groupdocs.com/display/parsernet/Get+document+info)
* [Detectar codificación](https://docs.groupdocs.com/display/parsernet/Detect+encoding)

### Ver también

* espacio de nombres [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* asamblea [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

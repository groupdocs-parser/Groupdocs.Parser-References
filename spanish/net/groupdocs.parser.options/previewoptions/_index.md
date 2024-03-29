---
title: PreviewOptions
second_title: Referencia de API de GroupDocs.Parser para .NET
description: Proporciona opciones para establecer requisitos y transmitir delegados para la generación de vista previa.
type: docs
weight: 570
url: /es/net/groupdocs.parser.options/previewoptions/
---
## PreviewOptions class

Proporciona opciones para establecer requisitos y transmitir delegados para la generación de vista previa.

```csharp
public class PreviewOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PreviewOptions](previewoptions#constructor)(CreatePageStream) | Inicializa una nueva instancia del[`PreviewOptions`](../previewoptions) clase que hace que se cierre el flujo de salida. |
| [PreviewOptions](previewoptions#constructor_1)(CreatePageStream, ReleasePageStream) | Inicializa una nueva instancia de[`PreviewOptions`](../previewoptions) class que hace que el flujo de salida se devuelva al cliente para su uso posterior. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CreatePageStream](../../groupdocs.parser.options/previewoptions/createpagestream) { get; set; } | Obtiene o establece una instancia del delegado de creación de flujo de páginas. |
| [Dpi](../../groupdocs.parser.options/previewoptions/dpi) { get; set; } | Obtiene o establece un dpi. |
| [Height](../../groupdocs.parser.options/previewoptions/height) { get; set; } | Obtiene o establece la altura de vista previa de la página. |
| [PageNumbers](../../groupdocs.parser.options/previewoptions/pagenumbers) { get; set; } | Obtiene o establece una matriz de números de página para generar vistas previas. |
| [PreviewFormat](../../groupdocs.parser.options/previewoptions/previewformat) { get; set; } | Obtiene o establece el formato de la imagen de vista previa. |
| [PreviewPageRender](../../groupdocs.parser.options/previewoptions/previewpagerender) { get; set; } | Obtiene o establece una instancia del delegado de información de procesamiento de vista previa de página. |
| [ReleasePageStream](../../groupdocs.parser.options/previewoptions/releasepagestream) { get; set; } | Obtiene o establece una instancia del delegado de finalización de vista previa de página. |
| [Width](../../groupdocs.parser.options/previewoptions/width) { get; set; } | Obtiene o establece el ancho de vista previa de la página. |

### Ver también

* espacio de nombres [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* asamblea [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

---
title: GroupDocs.Parser.Data
second_title: Referencia de API de GroupDocs.Parser para .NET
description: El espacio de nombres proporciona clases que representan los resultados del análisis.
type: docs
weight: 20
url: /es/net/groupdocs.parser.data/
---
El espacio de nombres proporciona clases que representan los resultados del análisis.

## Clases

| Clase | Descripción |
| --- | --- |
| [ContainerItem](./containeritem) | Representa un elemento contenedor como entidad de archivo Zip, archivo adjunto de correo electrónico, elemento de cartera PDF, etc. |
| [DocumentData](./documentdata) | Representa datos del documento. Consiste en[`FieldData`](../groupdocs.parser.data/fielddata)objects que contienen datos de campo de document. |
| [FieldData](./fielddata) | Representa datos de campo como un nombre, un índice de página, un valor de campo, etc. Según el campo, el valor puede ser un texto, una imagen, una tabla, etc. |
| [HighlightItem](./highlightitem) | Representa un resaltado, una parte del texto que generalmente se usa para explicar el contexto del texto encontrado en la funcionalidad de búsqueda. |
| [MetadataItem](./metadataitem) | Representa un elemento de metadatos que se utiliza en los elementos de contenedor y la funcionalidad de extracción de metadatos. |
| [Page](./page) | Representa la información de la página del documento, como el índice de página y el tamaño de página. Se usa para representar la página que contiene herederos de[`PageArea`](../groupdocs.parser.data/pagearea)class en la funcionalidad de análisis por plantilla. |
| [PageArea](./pagearea) | Representa una clase base abstracta para áreas de página que se utilizan para representar bloques en la página del documento en la funcionalidad de análisis por plantilla. |
| [PageBarcodeArea](./pagebarcodearea) | Representa un área de código de barras de página que se utiliza para representar un valor de código de barras en la funcionalidad de análisis por plantilla. |
| [PageGroupArea](./pagegrouparea) | Representa un grupo de áreas de página que se utiliza para agrupar diferentes tipos de bloques de la página del documento en la funcionalidad de análisis por plantilla. |
| [PageHyperlinkArea](./pagehyperlinkarea) | Representa un área de página que se utiliza para representar un hipervínculo en la página. |
| [PageImageArea](./pageimagearea) | Representa un área de imagen de página que se utiliza para representar una imagen en la página en la funcionalidad de análisis por plantilla o un archivo adjunto de imagen si las imágenes se extraen de correos electrónicos o archivos Zip. |
| [PageTableArea](./pagetablearea) | Representa un área de página de tabla que se utiliza para representar una tabla en la funcionalidad de análisis por plantilla. |
| [PageTableAreaCell](./pagetableareacell) | Representa una celda de tabla que se utiliza en[`PageTableArea`](../groupdocs.parser.data/pagetablearea) clase. |
| [PageTextArea](./pagetextarea) | Representa un área de texto de página que se utiliza para representar un valor de texto en la funcionalidad de análisis por plantilla o formulario de análisis. |
| [Point](./point) | Representa un punto. |
| [Rectangle](./rectangle) | Representa un área rectangular. |
| [SearchResult](./searchresult) | Representa el resultado de la búsqueda en la funcionalidad de búsqueda. |
| [Size](./size) | Representa un tamaño. |
| [TextStyle](./textstyle) | Representa el estilo del texto, como el nombre de la fuente, el tamaño de la fuente, etc. |
| [TocItem](./tocitem) | Representa el elemento que se utiliza en la funcionalidad de extracción de la tabla de contenido. |

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

---
title: TemplateLinkedPosition
second_title: Referencia de API de GroupDocs.Parser para .NET
description: Proporciona una posición de campo de plantilla que utiliza el campo vinculado.
type: docs
weight: 700
url: /es/net/groupdocs.parser.templates/templatelinkedposition/
---
## TemplateLinkedPosition class

Proporciona una posición de campo de plantilla que utiliza el campo vinculado.

```csharp
public sealed class TemplateLinkedPosition : TemplatePosition
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [TemplateLinkedPosition](templatelinkedposition#constructor)(string, Size, TemplateLinkedPositionEdges) | Inicializa una nueva instancia del[`TemplateLinkedPosition`](../templatelinkedposition) clase. |
| [TemplateLinkedPosition](templatelinkedposition#constructor_1)(string, Size, TemplateLinkedPositionEdges, bool) | Inicializa una nueva instancia del[`TemplateLinkedPosition`](../templatelinkedposition) clase. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AutoScale](../../groupdocs.parser.templates/templatelinkedposition/autoscale) { get; } | Obtiene el valor que indica si[`SearchArea`](./searcharea) está escalado por el tamaño del campo vinculado. |
| [Edges](../../groupdocs.parser.templates/templatelinkedposition/edges) { get; } | Obtiene los bordes del campo vinculado donde se busca un campo. |
| [LinkedFieldName](../../groupdocs.parser.templates/templatelinkedposition/linkedfieldname) { get; } | Obtiene el nombre del campo vinculado. |
| [SearchArea](../../groupdocs.parser.templates/templatelinkedposition/searcharea) { get; } | Obtiene el tamaño del área donde se busca un campo. |

### Ejemplos

El siguiente ejemplo muestra el código para la situación si se sabe que el campo con un número de factura se encuentra a la derecha de la cadena "Número de factura" se utiliza el siguiente código:

```csharp
// Crear un campo de plantilla de expresiones regulares para encontrar el texto "Número de factura"
TemplateField invoice = new TemplateField(new TemplateRegexPosition("Invoice Number"), "Invoice");

// Cree un campo de plantilla relacionado asociado con el campo "Factura" y extraiga el valor a la derecha del mismo
TemplateField invoiceNumber = new TemplateField(
    new TemplateLinkedPosition("invoice", new Size(100, 15), new TemplateLinkedPositionEdges(false, false, true, false)),
    "InvoiceNumber");
```

### Ver también

* class [TemplatePosition](../templateposition)
* espacio de nombres [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* asamblea [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

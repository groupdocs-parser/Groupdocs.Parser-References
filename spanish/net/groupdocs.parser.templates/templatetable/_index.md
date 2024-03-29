---
title: TemplateTable
second_title: Referencia de API de GroupDocs.Parser para .NET
description: Proporciona la tabla de plantilla.
type: docs
weight: 740
url: /es/net/groupdocs.parser.templates/templatetable/
---
## TemplateTable class

Proporciona la tabla de plantilla.

```csharp
public sealed class TemplateTable : TemplateItem
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [TemplateTable](templatetable#constructor)(TemplateTableLayout, string, int?) | Inicializa una nueva instancia del[`TemplateTable`](../templatetable) clase. |
| [TemplateTable](templatetable#constructor_1)(TemplateTableParameters, string, int?) | Inicializa una nueva instancia del[`TemplateTable`](../templatetable) clase. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Layout](../../groupdocs.parser.templates/templatetable/layout) { get; } | Obtiene el diseño de la tabla. |
| [Name](../../groupdocs.parser.templates/templateitem/name) { get; } | Obtiene el nombre del elemento de la plantilla. |
| [PageIndex](../../groupdocs.parser.templates/templateitem/pageindex) { get; } | Obtiene el índice de página del elemento de la plantilla. |
| [Parameters](../../groupdocs.parser.templates/templatetable/parameters) { get; } | Obtiene los parámetros para detectar la tabla en modo automático. |

### Observaciones

Hay dos formas de definir una tabla:

* Usando[`TemplateTableLayout`](../templatetablelayout) clase. En este caso la tabla se define por su posición en la página: área rectangular, columnas y separadores de filas.
* Usando[`TemplateTableParameters`](../templatetableparameters) class. En este caso la tabla es detectada automáticamente por algoritmos con parámetros establecidos. Ver[`TemplateTableParameters`](../templatetableparameters) clase para más información.

### Ver también

* class [TemplateItem](../templateitem)
* espacio de nombres [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* asamblea [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

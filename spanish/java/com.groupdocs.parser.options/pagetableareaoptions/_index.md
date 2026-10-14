---
title: "PageTableAreaOptions"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona las opciones que se utilizan para la extracción de áreas de tabla de página."
type: docs
weight: 31
url: /es/java/com.groupdocs.parser.options/pagetableareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTableAreaOptions extends PageAreaOptions
```

Proporciona las opciones que se utilizan para la extracción de áreas de tabla de página.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [PageTableAreaOptions(TemplateTableLayout tableLayout)](#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-) | Inicializa una nueva instancia de la clase [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions). |
|
|  | [PageTableAreaOptions(Rectangle rectangle)](#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-) | Inicializa una nueva instancia de la clase [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) con un rectángulo de búsqueda y sin diseño fijo. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getTableLayout()](#getTableLayout--) | Obtiene el diseño de tabla que define la tabla en una página. |
|
### PageTableAreaOptions(TemplateTableLayout tableLayout) {#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-}
```
public PageTableAreaOptions(TemplateTableLayout tableLayout)
```


Inicializa una nueva instancia de la clase [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | tableLayout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | El diseño de tabla que define la tabla en una página. |
|

### PageTableAreaOptions(Rectangle rectangle) {#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageTableAreaOptions(Rectangle rectangle)
```


Inicializa una nueva instancia de la clase [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) con un rectángulo de búsqueda y sin diseño fijo.

Útil para restringir las tablas detectadas automáticamente a una región de la página. Refleja el C#

new PageTableAreaOptions(null) { Rectangle = ... }
patrón.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular en la página donde se deben detectar las tablas; pase  null  para buscar en toda la página. |
|

### getTableLayout() {#getTableLayout--}
```
public TemplateTableLayout getTableLayout()
```


Obtiene el diseño de tabla que define la tabla en una página.


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instane of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class.


---
title: Parser
second_title: Referencia de API de GroupDocs.Parser para .NET
description: Representa la clase principal que controla el texto las imágenes la extracción de contenedores y la funcionalidad de análisis.
type: docs
weight: 590
url: /es/net/groupdocs.parser/parser/
---
## Parser class

Representa la clase principal que controla el texto, las imágenes, la extracción de contenedores y la funcionalidad de análisis.

```csharp
public sealed class Parser : IDisposable
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | Inicializa una nueva instancia del[`Parser`](../parser) clase para extraer datos de una base de datos. |
| [Parser](parser#constructor)(EmailConnection) | Inicializa una nueva instancia del[`Parser`](../parser) clase para extraer datos de un servidor de correo electrónico remoto. |
| [Parser](parser#constructor_4)(Stream) | Inicializa una nueva instancia del[`Parser`](../parser) clase. |
| [Parser](parser#constructor_7)(string) | Inicializa una nueva instancia del[`Parser`](../parser) clase. |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | Inicializa una nueva instancia del[`Parser`](../parser) clase para extraer datos de una base de datos. |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | Inicializa una nueva instancia del[`Parser`](../parser) clase para extraer datos de un servidor de correo electrónico remoto. |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | Inicializa una nueva instancia del[`Parser`](../parser) clase con[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_8)(string, LoadOptions) | Inicializa una nueva instancia del[`Parser`](../parser) clase con[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | Inicializa una nueva instancia del[`Parser`](../parser) clase con[`LoadOptions`](../../groupdocs.parser.options/loadoptions) y[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_9)(string, LoadOptions, ParserSettings) | Inicializa una nueva instancia del[`Parser`](../parser) clase con[`LoadOptions`](../../groupdocs.parser.options/loadoptions) y[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | Obtiene las funciones admitidas. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | Realiza tareas definidas por la aplicación asociadas con liberar, liberar o restablecer recursos no administrados. |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | Obtener vista previa de páginas. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | Extrae códigos de barras del documento. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_2)(int) | Extrae códigos de barras de la página del documento. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(PageAreaOptions) | Extrae códigos de barras del documento usando las opciones de personalización (para configurar el área rectangular que contiene códigos de barras). |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int, PageAreaOptions) | Extrae códigos de barras de la página del documento usando las opciones de personalización (para establecer el área rectangular que contiene códigos de barras). |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | Extrae un objeto contenedor del documento para trabajar con formatos que contienen archivos adjuntos, archivos ZIP, etc. |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | Devuelve la información general sobre el documento. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | Extrae un texto formateado del documento. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | Extrae un texto formateado de la página del documento. |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | Extrae un resaltado del documento. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | Extrae hipervínculos del documento. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | Extrae hipervínculos de la página del documento. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | Extrae los hipervínculos del documento usando las opciones de personalización (para establecer el área rectangular que contiene los hipervínculos). |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | Extrae hipervínculos de la página del documento usando las opciones de personalización (para establecer el área rectangular que contiene los hipervínculos). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | Extrae imágenes del documento. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | Extrae imágenes de la página del documento. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | Extrae imágenes del documento usando las opciones de personalización (para establecer el área rectangular que contiene las imágenes). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | Extrae imágenes de la página del documento usando las opciones de personalización (para establecer el área rectangular que contiene las imágenes). |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | Extrae metadatos del documento. |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | Extrae un texto estructurado del documento. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)(PageTableAreaOptions) | Extrae tablas del documento. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(int, PageTableAreaOptions) | Extrae tablas de la página del documento. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | Extrae un texto del documento. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | Extrae un texto de la página del documento. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | Extrae una página de texto del documento usando las opciones de texto (para habilitar el modo de extracción rápida de texto sin formato). |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | Extrae un texto de la página del documento usando las opciones de texto (para habilitar el modo de extracción rápida de texto sin formato). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | Extrae áreas de texto del documento. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | Extrae áreas de texto de la página del documento. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | Extrae áreas de texto del documento usando opciones de personalización (expresión regular, mayúsculas y minúsculas, etc.). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | Extrae áreas de texto de la página del documento usando opciones de personalización (expresión regular, mayúsculas y minúsculas, etc.). |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | Extrae una tabla de contenido del documento. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate)(Template) | Analiza el documento según la plantilla generada por el usuario. |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | Analiza el formulario del documento. |
| [Search](../../groupdocs.parser/parser/search#search)(string) | Busca un*keyword* en el documento. |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | Busca un*keyword*en el documento usando las opciones de búsqueda (expresión regular, mayúsculas y minúsculas, etc.). |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | Devuelve la información general sobre un archivo. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | Devuelve la información general sobre un archivo. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | Devuelve la información general sobre un archivo. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | Devuelve la información general sobre un archivo. |

### Ver también

* espacio de nombres [GroupDocs.Parser](../../groupdocs.parser)
* asamblea [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->

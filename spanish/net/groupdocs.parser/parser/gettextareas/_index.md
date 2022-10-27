---
title: GetTextAreas
second_title: Referencia de API de GroupDocs.Parser para .NET
description: Extrae áreas de texto del documento.
type: docs
weight: 160
url: /es/net/groupdocs.parser/parser/gettextareas/
---
## GetTextAreas() {#gettextareas}

Extrae áreas de texto del documento.

```csharp
public IEnumerable<PageTextArea> GetTextAreas()
```

### Valor_devuelto

Una colección de[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objetos; `nulo` si la extracción de áreas de texto no es compatible.

### Observaciones

**Aprende más:**

* [Extraer áreas de texto](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Ejemplos

El siguiente ejemplo muestra cómo extraer todas las áreas de texto de todo el documento:

```csharp
// Crea una instancia de la clase Parser
using(Parser parser = new Parser(filePath))
{
    // Extraer áreas de texto
    IEnumerable<PageTextArea> areas = parser.GetTextAreas();
    // Comprobar si se admite la extracción de áreas de texto
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Iterar sobre las áreas de texto de la página
    foreach(PageTextArea a in areas)
    {
        // Imprimir un valor de índice de página, rectángulo y área de texto:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Ver también

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## GetTextAreas(PageTextAreaOptions) {#gettextareas_1}

Extrae áreas de texto del documento usando opciones de personalización (expresión regular, mayúsculas y minúsculas, etc.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(PageTextAreaOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| options | PageTextAreaOptions | Las opciones para la extracción del área de texto. |

### Valor_devuelto

Una colección de[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objetos; `nulo` si la extracción de áreas de texto no es compatible.

### Observaciones

**Aprende más:**

* [Extraer áreas de texto](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Ejemplos

El siguiente ejemplo muestra cómo extraer solo áreas de texto con dígitos de la esquina superior izquierda:

```csharp
// Crea una instancia de la clase Parser
using(Parser parser = new Parser(filePath))
{
    // Crear las opciones que se utilizan para la extracción del área de texto
    PageTextAreaOptions options = new PageTextAreaOptions("[0-9]+", new Rectangle(new Point(0, 0), new Size(300, 100)));

    // Extrae áreas de texto que contienen solo dígitos de la esquina superior izquierda de una página:
    IEnumerable<PageTextArea> areas = parser.GetTextAreas(options);
    // Comprobar si se admite la extracción de áreas de texto
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Iterar sobre las áreas de texto de la página
    foreach(PageTextArea a in areas)
    {
        // Imprimir un valor de índice de página, rectángulo y área de texto:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Ver también

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## GetTextAreas(int) {#gettextareas_2}

Extrae áreas de texto de la página del documento.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pageIndex | Int32 | El índice de página de base cero. |

### Valor_devuelto

Una colección de[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objetos; `nulo` si la extracción de áreas de texto no es compatible.

### Observaciones

**Aprende más:**

* [Extraer áreas de texto](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Ejemplos

Para extraer áreas de texto de una página de documento se utiliza el siguiente método:

```csharp
// Crea una instancia de la clase Parser
using(Parser parser = new Parser(filePath))
{
    // Comprobar si el documento admite la extracción de áreas de texto
    if(!parser.Features.TextAreas)
    {
        Console.WriteLine("Document isn't supports text areas extraction.");
        return;
    }

    // Obtener la información del documento
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Comprobar si el documento tiene páginas
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Iterar sobre páginas
    for(int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Imprimir un número de página 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
 
        // Iterar sobre las áreas de texto de la página
        // Ignoramos la verificación nula ya que hemos verificado la compatibilidad con la función de extracción de áreas de texto anteriormente
        foreach(PageTextArea a in parser.GetTextAreas(pageIndex))
        {
            // Imprime un rectángulo y un valor de área de texto:
            Console.WriteLine(string.Format("R: {0}, Text: {1}", a.Rectangle, a.Text));
        }
    }
}
```

### Ver también

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## GetTextAreas(int, PageTextAreaOptions) {#gettextareas_3}

Extrae áreas de texto de la página del documento usando opciones de personalización (expresión regular, mayúsculas y minúsculas, etc.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex, PageTextAreaOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pageIndex | Int32 | El índice de página de base cero. |
| options | PageTextAreaOptions | Las opciones para la extracción del área de texto. |

### Valor_devuelto

Una colección de[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objetos; `nulo` si la extracción de áreas de texto no es compatible.

### Observaciones

**Aprende más:**

* [Extraer áreas de texto](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Ver también

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
